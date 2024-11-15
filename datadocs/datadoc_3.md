---
archived: false
created_at: '2024-11-15T20:17:15'
environment_id: 1
id: 3
meta:
  variables: []
owner_uid: 1
public: true
title: Sampling Demo
updated_at: '2024-11-15T20:27:06'
---

# Sampling Demo

<!--
cell_type: query
created_at: '2024-11-15T20:17:15'
id: 34
meta:
  engine: 1
  title: Select Test Results from Code Quality History
updated_at: '2024-11-15T20:17:37'
-->
## Query: Select Test Results from Code Quality History

```sql
-- Sample query selecting some columns from the code_quality.test_result_history table
SELECT 
    repository, 
    test_short_name, 
    duration_s, 
    status, 
    attempts 
FROM 
    code_quality.test_result_history 
LIMIT 10;
```


<!--
cell_type: query
created_at: '2024-11-15T20:17:39'
id: 35
meta:
  engine: 1
updated_at: '2024-11-15T20:17:39'
-->
## Query: Query

```sql

```


<!--
cell_type: query
created_at: '2024-11-15T20:17:40'
id: 36
meta:
  engine: 1
updated_at: '2024-11-15T20:17:40'
-->
## Query: Query

```sql

```


<!--
cell_type: query
created_at: '2024-11-15T20:17:41'
id: 37
meta:
  engine: 1
updated_at: '2024-11-15T20:17:41'
-->
## Query: Query

```sql

```


<!--
cell_type: text
created_at: '2024-11-15T20:17:42'
id: 38
meta:
  collapsed: false
updated_at: '2024-11-15T20:17:50'
-->
## Text

<p><br></p>


<!--
cell_type: chart
created_at: '2024-11-15T20:17:43'
id: 39
meta:
  chart:
    type: line
    x_axis:
      col_idx: 0
      label: ''
    y_axis:
      label: ''
      series: {}
  collapsed: false
  data:
    source_type: cell_above
    transformations:
      format: {}
  title: ''
  visual: {}
updated_at: '2024-11-15T20:17:43'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: query
created_at: '2024-11-15T20:17:45'
id: 40
meta:
  engine: 1
updated_at: '2024-11-15T20:17:56'
-->
## Query: Query

```sql
set session pinterest_query_category = 'expensive';

SELECT dt, count(1) as cnt

FROM default.safe_mobile_json_log

where 
  dt BETWEEN '2024-10-08' and '2024-10-08'  
  
  
group by 1 limit 1000;
```


<!--
cell_type: query
created_at: '2024-11-15T20:17:57'
id: 41
meta:
  engine: 1
  title: Fetch fefUnique Timestamps from 2024 Onwards
updated_at: '2024-11-15T20:18:08'
-->
## Query: Fetch fefUnique Timestamps from 2024 Onwards

```sql
SELECT
  time
FROM default_bdp_sampled.safe_frontend_impression_event
WHERE
  dt >= '2024-01-01'
GROUP BY
  1
LIMIT 1000;
```


<!--
cell_type: query
created_at: '2024-11-15T20:26:55'
id: 49
meta:
  engine: 1
  title: Retrieve Sampled Table Names
updated_at: '2024-11-15T20:27:06'
-->
## Query: Retrieve Sampled Table Names

```sql
SELECT
  table_name,
  sampled_table_name
FROM
  bi_internal.sampled_tables
```


<!--
cell_type: query
created_at: '2024-11-15T20:18:07'
id: 42
meta:
  engine: 1
  title: Compare Full vs Sampled Data Impressions and Repins
updated_at: '2024-11-15T20:18:18'
-->
## Query: Compare Full vs Sampled Data Impressions and Repins

```sql
SET spark.driver.memory=16G;
SET spark.executor.cores=2;
SET spark.executor.memory=16G;
SET spark.executor.memoryOverhead=4G;
SET spark.dynamicAllocation.maxExecutors=1000;
with all_data (
select dt, sum(num_impressions) num_impressions, sum(num_repins) num_repins
from bi.core_daily_feedview_pin_stats
where dt >= '2023-09-01' and dt <= '2024-03-31'
group by 1
),

sampled (
select dt,sum(num_impressions) num_impressions, sum(num_repins) num_repins
from bi_bdp_sampled.core_daily_feedview_pin_stats
where dt >= '2023-09-01' and dt <= '2024-03-31'
group by 1
)

select 
  a.dt,
  a.num_repins as all_data_num_repins,
  b.num_repins*100 as sampled_data_num_repins_upscaled,
  a.num_impressions as all_data_num_impressions,
  b.num_impressions*100 as sampled_data_num_impressions_upscaled,
  (b.num_impressions*100.00 - a.num_impressions) / a.num_impressions as num_impressions_error,
  (b.num_repins*100.00 - a.num_repins) / a.num_repins as num_repins_error
from all_data a 
  inner join sampled b on a.dt = b.dt
order by a.dt desc limit 1000;
```


<!--
cell_type: query
created_at: '2024-11-15T20:18:18'
id: 43
meta:
  engine: 1
updated_at: '2024-11-15T20:18:26'
-->
## Query: Query

```sql
/* Query to find the top pinners based on their engagement metrics over the last 90 days */
SELECT userId, 
       pinnability__root_pinner__numClickthroughsFromLast90Days, 
       pinnability__root_pinner__numGridClicksFromLast90Days, 
       pinnability__root_pinner__numOtherCloseupsFromLast90Days, 
       pinnability__root_pinner__numRepinsFromLast90Days
FROM galaxy_user_features.root_pinner_pinnability_stats_90days
ORDER BY pinnability__root_pinner__numClickthroughsFromLast90Days DESC, 
         pinnability__root_pinner__numGridClicksFromLast90Days DESC, 
         pinnability__root_pinner__numOtherCloseupsFromLast90Days DESC, 
         pinnability__root_pinner__numRepinsFromLast90Days DESC
LIMIT 10;
```
