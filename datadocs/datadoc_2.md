---
archived: false
created_at: 2024-10-07 19:31:42
environment_id: 1
id: 2
meta:
  variables: []
owner_uid: 2
public: true
title: Title 6
updated_at: 2024-10-21 18:13:59
---

# Title 6

---
cell_type: query
created_at: 2024-10-07 19:31:42
id: 14
meta:
  engine: 1
  title: query title 6
updated_at: 2024-10-21 18:13:59
---
```query
SELECT
  time
FROM default_bdp_sampled.safe_frontend_impression_event
WHERE
  dt >= '2024-01-01'
GROUP BY
  1
LIMIT 1000;
```

---
cell_type: text
created_at: 2024-10-11 19:58:02
id: 15
meta:
  collapsed: false
updated_at: 2024-10-15 16:32:58
---
```text
<p>SOME TEXT 6</p>
```

---
cell_type: chart
created_at: 2024-10-15 15:32:08
id: 18
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
updated_at: 2024-10-15 15:32:08
---
```chart

```

---
cell_type: chart
created_at: 2024-10-15 15:32:07
id: 17
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
updated_at: 2024-10-15 15:32:07
---
```chart

```

---
cell_type: chart
created_at: 2024-10-11 21:56:46
id: 16
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
updated_at: 2024-10-11 21:56:46
---
```chart

```