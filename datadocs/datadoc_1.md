---
archived: false
created_at: '2024-11-13T00:40:39'
environment_id: 1
id: 1
meta:
  variables:
  - name: Region
    type: string
    value: Western Europe
owner_uid: 1
public: true
title: World Happiness Report (2015-2019)
updated_at: '2024-11-13T18:58:26'
---

# World Happiness Report (2015-2019)

<!--
cell_type: query
created_at: '2024-11-13T17:13:53'
id: 14
meta:
  engine: 1
  title: Western Europe Countries Ranking
updated_at: '2024-11-13T18:58:26'
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
  world_happiness_ranking_2015_to_2019
WHERE Region = "{{Region}}";
```


<!--
cell_type: chart
created_at: '2024-11-13T17:13:53'
id: 15
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
updated_at: '2024-11-13T17:13:53'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: chart
created_at: '2024-11-13T17:13:53'
id: 16
meta:
  chart:
    type: line
    x_axis:
      col_idx: 0
      label: Year
      sort:
        asc: true
        idx: 0
    y_axis:
      label: Rank
      series:
        '0':
          agg_type: sum
        '1':
          agg_type: sum
        '10':
          agg_type: sum
        '11':
          agg_type: sum
        '12':
          agg_type: sum
        '13':
          agg_type: sum
        '14':
          agg_type: sum
        '15':
          agg_type: sum
        '16':
          agg_type: sum
        '17':
          agg_type: sum
        '18':
          agg_type: sum
        '19':
          agg_type: sum
        '2':
          agg_type: sum
        '20':
          agg_type: sum
        '3':
          agg_type: sum
        '4':
          agg_type: sum
        '5':
          agg_type: sum
        '6':
          agg_type: sum
        '7':
          agg_type: sum
        '8':
          agg_type: sum
        '9':
          agg_type: sum
      stack: false
  collapsed: false
  data:
    source_type: cell_above
    transformations:
      aggregate: false
      format: {}
      switch: true
  title: Western Europe Countries Ranking
  visual:
    legend_position: top
updated_at: '2024-11-13T17:13:53'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: chart
created_at: '2024-11-13T17:13:53'
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
updated_at: '2024-11-13T17:13:53'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: query
created_at: '2024-11-13T17:13:53'
id: 18
meta:
  engine: 1
  title: 2019 Top 10 Countries
updated_at: '2024-11-13T17:13:53'
-->
## Query: 2019 Top 10 Countries

```sql
SELECT
    Country,
    GDP,
    SocialSupport,
    HealthyLifeExpectancy,
    FreedomToMakeLifeChoices,
    Generosity,
    PerceptionsOfCorruption
FROM
    world_happiness_2019
LIMIT
    10;
```


<!--
cell_type: text
created_at: '2024-11-13T17:13:53'
id: 19
meta:
  collapsed: false
updated_at: '2024-11-13T17:13:53'
-->
## Text

<h1>title</h1>
<h2>subtitle</h2>
<ul>
  <li>bullet points</li>
</ul>
<ol>
  <li>List</li>
</ol>
<blockquote>Quote</blockquote>
<p><a href="link.com">Link</a></p>


<!--
cell_type: chart
created_at: '2024-11-13T17:13:53'
id: 20
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
updated_at: '2024-11-13T17:13:53'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: text
created_at: '2024-11-13T17:13:53'
id: 21
meta:
  collapsed: false
updated_at: '2024-11-13T17:13:53'
-->
## Text

<h2>Chart Cell: Bar Charts</h2>
<p>You can title, label<a href="fqwfwqf">, and configure the chart to display the results in an easy-to-understand manner.</a></p>
<blockquote><a href="fqwfwqf">Click on `CONFIG CHART` to see the chart settings </a>&amp; explore.</blockquote>
<blockquote><br></blockquote>
<blockquote>ffqwf</blockquote>


<!--
cell_type: text
created_at: '2024-11-13T17:13:53'
id: 22
meta:
  collapsed: false
updated_at: '2024-11-13T17:13:53'
-->
## Text

<p>qfqwfwq</p>


<!--
cell_type: chart
created_at: '2024-11-13T17:13:53'
id: 23
meta:
  chart:
    type: bar
    x_axis:
      col_idx: 0
      label: Categories
    y_axis:
      label: Score
      series:
        '0':
          agg_type: sum
        '1':
          agg_type: sum
        '10':
          agg_type: sum
        '2':
          agg_type: sum
        '3':
          agg_type: sum
        '4':
          agg_type: sum
        '5':
          agg_type: sum
        '6':
          agg_type: sum
        '7':
          agg_type: sum
        '8':
          agg_type: sum
        '9':
          agg_type: sum
      stack: false
  collapsed: false
  data:
    source_type: cell_above
    transformations:
      aggregate: false
      format: {}
      switch: true
  title: 2019 Top 10 Countries
  visual:
    legend_position: top
updated_at: '2024-11-13T17:13:53'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: text
created_at: '2024-11-13T17:13:53'
id: 24
meta:
  collapsed: false
updated_at: '2024-11-13T17:13:53'
-->
## Text

{"blocks":[{"key":"cbs69","text":"Query Cell","type":"header-two","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"5ajp","text":"The query cell below has been collapsed. ","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"bvfr2","text":"Query cells can be collapsed in order to make DataDocs easier to view.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"2d2q7","text":"","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"f24oq","text":"Hover over the title Top 10 Countries Score to see the cell management buttons.","type":"unstyled","depth":0,"inlineStyleRanges":[{"offset":21,"length":22,"style":"ITALIC"}],"entityRanges":[],"data":{}},{"key":"4kip1","text":"Click on the dropdown button on the top left or on the cell itself to uncollapse the cell and run the query. ","type":"unstyled","depth":0,"inlineStyleRanges":[{"offset":48,"length":11,"style":"BOLD"}],"entityRanges":[],"data":{}},{"key":"c0c7","text":"You can click on the lock button that appears next to the dropdown button to change the default setting of the cell when the DataDoc loads.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}}],"entityMap":{}}


<!--
cell_type: query
created_at: '2024-11-13T17:13:53'
id: 25
meta:
  collapsed: false
  engine: 1
  title: Top 10 Countries Score
updated_at: '2024-11-13T17:13:53'
-->
## Query: Top 10 Countries Score

```sql
{% macro query(year) %}
{% set rank = 'Rank' if year > 2017 else 'HappinessRank' %}
{% set score = 'Score' if year > 2017 else 'HappinessScore as Score' %}
SELECT
  *
FROM(
    SELECT
      '{{ year }}' AS Year,
      Country,
      {{ score }}
    FROM
      world_happiness_{{year}}
    ORDER BY
      {{ rank }}
    LIMIT
      10
  )
{%- endmacro %}
{% for i in [2019, 2018, 2017, 2016, 2015] %}
  {% if loop.index0 != 0 %}
    UNION
  {% endif %}
  {{ query(i) }}
{% endfor %}
ORDER BY
Score DESC;
  -- This is another example of templating!
  -- Check out: https://jinja.palletsprojects.com/en/2.11.x/templates/
  --    for more usages and information!
```


<!--
cell_type: text
created_at: '2024-11-13T17:13:53'
id: 26
meta:
  collapsed: false
updated_at: '2024-11-13T17:13:53'
-->
## Text

{"blocks":[{"key":"ds1ln","text":"Chart Cells: Multiple Charts from Results","type":"header-two","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"3opak","text":"The results from a query cell can be manipulated to visualize the data in different ways.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"cnu9f","text":"Below are two examples of the same data.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"anuvc","text":"Check out the configurations to see how the data was transformed.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}}],"entityMap":{}}


<!--
cell_type: chart
created_at: '2024-11-13T17:13:53'
id: 27
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
updated_at: '2024-11-13T17:13:53'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: text
created_at: '2024-11-13T17:13:53'
id: 28
meta:
  collapsed: false
updated_at: '2024-11-13T17:13:53'
-->
## Text

<h2>Query Cell</h2>
<p>Here is another query for you to run!</p>
<p>TTGEGWEGWEG</p>


<!--
cell_type: text
created_at: '2024-11-13T17:13:53'
id: 29
meta:
  collapsed: false
updated_at: '2024-11-13T17:13:53'
-->
## Text

<h2>Query Cell</h2>
<p>Here is another query for you to run!</p>
<p>TheGWEGWEGWEGe Query Editor.</p>


<!--
cell_type: text
created_at: '2024-11-13T17:13:53'
id: 30
meta:
  collapsed: false
updated_at: '2024-11-13T17:13:53'
-->
## Text

<h2><del><u><em>fasfwqfqwffqwf</em></u></del></h2>
<h2><br></h2>
<h2><del><u><em>f</em></u></del></h2>
<h2><del><u><em>qwfqw</em></u></del></h2>
<h2><del><u><em>f</em></u></del></h2>
<h2><del><u><em>qwqwfqwfwqqw</em></u></del></h2>
<p><br></p>
<ol>
  <li><a href="fqf">qf</a></li>
</ol>
<blockquote><a href="fqf">qfqwfqw</a></blockquote>


<!--
cell_type: chart
created_at: '2024-11-13T17:13:53'
id: 31
meta:
  chart:
    type: bar
    x_axis:
      col_idx: 0
      label: Country
    y_axis:
      label: Happiness Score
      series:
        '0':
          agg_type: sum
        '1':
          agg_type: sum
          color: 1
        '2':
          agg_type: sum
          color: 5
        '3':
          agg_type: sum
        '4':
          agg_type: sum
          color: 6
        '5':
          agg_type: sum
          color: 9
      stack: false
  collapsed: false
  data:
    source_type: cell_above
    transformations:
      aggregate: true
      format:
        agg_col: 1
        series_col: 0
        value_cols:
        - 2
      switch: false
  title: Top 10 Countries Score
  visual:
    legend_position: top
updated_at: '2024-11-13T17:13:53'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: chart
created_at: '2024-11-13T17:13:53'
id: 32
meta:
  chart:
    type: histogram
    x_axis:
      col_idx: 0
      label: Year
    y_axis:
      label: Happiness Score
      series:
        '0':
          agg_type: sum
        '1':
          agg_type: sum
          color: 12
        '10':
          agg_type: sum
          color: 11
        '11':
          agg_type: sum
          color: 2
        '2':
          agg_type: sum
          color: 5
        '3':
          agg_type: sum
          color: 14
        '4':
          agg_type: sum
          color: 3
        '5':
          agg_type: sum
          color: 13
        '6':
          agg_type: sum
          color: 6
        '7':
          agg_type: sum
          color: 9
        '8':
          agg_type: sum
          color: 0
        '9':
          agg_type: sum
          color: 4
      stack: false
  collapsed: false
  data:
    source_type: cell_above
    transformations:
      aggregate: true
      format:
        agg_col: 0
        series_col: 1
        value_cols:
        - 2
      switch: false
  title: Top 10 Countries Score
  visual:
    legend_position: top
updated_at: '2024-11-13T17:13:53'
-->
## Chart

*Chart generated from the metadata.*
