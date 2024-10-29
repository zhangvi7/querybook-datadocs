---
archived: false
created_at: '2024-10-28T14:23:42'
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
updated_at: '2024-10-29T03:48:19'
---

# World Happiness Report (2015-2019)

<!--
cell_type: text
created_at: '2024-10-28T14:23:42'
id: 1
meta:
  collapsed: false
updated_at: '2024-10-28T20:37:10'
-->
<h1>Welcome to Querybook!&nbsp;</h1>
<p>This is a demo DataDoc.</p>
<p>Below are some pre-filled cells for you to interact with.</p>
<p><br></p>
<p>This is a text cell thafqwfqwft can be used for creating narratives and note-taking.</p>
<p><br></p>
<p>First, click on the Tables section in the left sidebar to look at the tables we have.</p>
<p>Click on any table and on <strong>VIEW TABLE</strong> to inspectgqwgthe <strong>Lineage</strong> tab.</p>
<p><br></p>
<p>Now, let us get started by clicking on the run button in the query cell below.</p>


<!--
cell_type: text
created_at: '2024-10-28T20:36:38'
id: 14
meta:
  collapsed: false
updated_at: '2024-10-28T20:36:43'
-->
<p><br></p>


<!--
cell_type: query
created_at: '2024-10-28T14:23:42'
id: 2
meta:
  engine: 1
  title: qwWestern Europe Countries Ranking
updated_at: '2024-10-28T20:37:09'
-->
## Query: qwWestern Europe Countries Ranking

```sql
SELECT
  Country,4124
  Rank2015 AS [2015],
  Rank2016 AS [2016],
  Rank2017 AS [2017],
  Rank2018 ASfqwfqwf [2018],rqwrfwqfqwf
  Rank2019 AS [2019]
FROMfqfgqwf
  world_happiness_ranking_2015_to_2019
WHERE Region = "{{Region}}";
-- Region is a template variable with the value of 'Western Europe'
-- click on the <> button on the bottom right of the DataDoc to configure more!
```


<!--
cell_type: text
created_at: '2024-10-28T14:23:42'
id: 3
meta:
  collapsed: false
updated_at: '2024-10-28T14:23:42'
-->
{"blocks":[{"key":"ahup0","text":"Chart Cell: Line Graph","type":"header-two","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"tlat","text":"The settings on the chart below has been pre-set to display the results from the query cell above.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"vnl1","text":"","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"at9lo","text":"Hover over the chart to see the values in the tooltip.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}}],"entityMap":{}}


<!--
cell_type: chart
created_at: '2024-10-28T14:23:42'
id: 4
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
updated_at: '2024-10-28T14:23:42'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: text
created_at: '2024-10-28T14:23:42'
id: 5
meta:
  collapsed: false
updated_at: '2024-10-28T14:23:42'
-->
{"blocks":[{"key":"4pmfj","text":"Query Cell","type":"header-two","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"9c5lj","text":"Here is another query for you to run!","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"cooab","text":"The results can be shared with other users or exported.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"7nfpk","text":"Check out the controls on the bottom right of the Query Editor.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}}],"entityMap":{}}


<!--
cell_type: query
created_at: '2024-10-28T14:23:42'
id: 6
meta:
  engine: 1
  title: 2019 Top 10 Countries
updated_at: '2024-10-28T14:23:42'
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
created_at: '2024-10-29T03:48:08'
id: 17
meta:
  collapsed: false
updated_at: '2024-10-29T03:48:19'
-->
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
created_at: '2024-10-29T00:09:15'
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
updated_at: '2024-10-29T00:09:15'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: text
created_at: '2024-10-28T14:23:42'
id: 7
meta:
  collapsed: false
updated_at: '2024-10-29T03:42:56'
-->
<h2>Chart Cell: Bar Charts</h2>
<p>You can title, label<a href="fqwfwqf">, and configure the chart to display the results in an easy-to-understand manner.</a></p>
<blockquote><a href="fqwfwqf">Click on `CONFIG CHART` to see the chart settings </a>&amp; explore.</blockquote>
<blockquote><br></blockquote>
<blockquote>ffqwf</blockquote>


<!--
cell_type: text
created_at: '2024-10-29T00:09:32'
id: 16
meta:
  collapsed: false
updated_at: '2024-10-29T00:09:39'
-->
<p>qfqwfwq</p>


<!--
cell_type: chart
created_at: '2024-10-28T14:23:42'
id: 8
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
updated_at: '2024-10-28T14:23:42'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: text
created_at: '2024-10-28T14:23:42'
id: 9
meta:
  collapsed: false
updated_at: '2024-10-28T14:23:42'
-->
{"blocks":[{"key":"cbs69","text":"Query Cell","type":"header-two","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"5ajp","text":"The query cell below has been collapsed. ","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"bvfr2","text":"Query cells can be collapsed in order to make DataDocs easier to view.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"2d2q7","text":"","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"f24oq","text":"Hover over the title Top 10 Countries Score to see the cell management buttons.","type":"unstyled","depth":0,"inlineStyleRanges":[{"offset":21,"length":22,"style":"ITALIC"}],"entityRanges":[],"data":{}},{"key":"4kip1","text":"Click on the dropdown button on the top left or on the cell itself to uncollapse the cell and run the query. ","type":"unstyled","depth":0,"inlineStyleRanges":[{"offset":48,"length":11,"style":"BOLD"}],"entityRanges":[],"data":{}},{"key":"c0c7","text":"You can click on the lock button that appears next to the dropdown button to change the default setting of the cell when the DataDoc loads.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}}],"entityMap":{}}


<!--
cell_type: query
created_at: '2024-10-28T14:23:42'
id: 10
meta:
  collapsed: false
  engine: 1
  title: Top 10 Countries Score
updated_at: '2024-10-28T14:23:42'
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
created_at: '2024-10-28T14:23:42'
id: 11
meta:
  collapsed: false
updated_at: '2024-10-28T14:23:42'
-->
{"blocks":[{"key":"ds1ln","text":"Chart Cells: Multiple Charts from Results","type":"header-two","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"3opak","text":"The results from a query cell can be manipulated to visualize the data in different ways.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"cnu9f","text":"Below are two examples of the same data.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}},{"key":"anuvc","text":"Check out the configurations to see how the data was transformed.","type":"unstyled","depth":0,"inlineStyleRanges":[],"entityRanges":[],"data":{}}],"entityMap":{}}


<!--
cell_type: chart
created_at: '2024-10-28T14:23:42'
id: 12
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
updated_at: '2024-10-28T14:23:42'
-->
## Chart

*Chart generated from the metadata.*


<!--
cell_type: chart
created_at: '2024-10-28T14:23:42'
id: 13
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
updated_at: '2024-10-28T14:23:42'
-->
## Chart

*Chart generated from the metadata.*
