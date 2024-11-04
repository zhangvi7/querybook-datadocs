---
archived: false
created_at: '2024-11-01T18:31:49'
environment_id: 1
id: 5
meta:
  variables:
  - name: Region
    type: string
    value: Western Europe
owner_uid: 1
public: true
title: Sample datadoc title
updated_at: '2024-11-04T15:53:25'
---

# Sample datadoc title

<!--
cell_type: query
created_at: '2024-11-01T18:31:49'
id: 31
meta:
  engine: 1
  title: Western Europe Countries Ranking
updated_at: '2024-11-04T15:53:17'
-->
## Query: Western Europe Countries Ranking

```sql
SELECT
  Country,
  Rank2015 AS [2015],
  Rank2016 AS [2016],
  Rank2017 AS [2017],
  Rank2018 AS [2018],
  Rank2019 AS [2019]
FROM
  main.world_happiness_2017
WHERE Region = "{{Region}}";
```


<!--
cell_type: text
created_at: '2024-11-04T15:50:36'
id: 32
meta:
  collapsed: false
updated_at: '2024-11-04T15:53:25'
-->
## Text

<p>new text blha blha feff23f</p>


<!--
cell_type: text
created_at: '2024-11-04T15:51:28'
id: 34
meta:
  collapsed: false
updated_at: '2024-11-04T15:51:56'
-->
## Text

<p><strong>More text cell Content bold</strong></p>
<p>regular text here</p>
<p><em>italic text</em></p>
<p><br></p>


<!--
cell_type: chart
created_at: '2024-11-04T15:50:41'
id: 33
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
updated_at: '2024-11-04T15:50:41'
-->
## Chart

Chart generated from metadata
