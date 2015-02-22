---
title       : Comparing US statistics
subtitle    : Using State divisions and States to compare Data
author      : AudioChick
job         : Analytical Programmer
logo        : poct-logo.png
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax, quiz, bootstrap]
ext_widgets : {rCharts: ["libraries/highcharts","libraries/nvd3", "libraries/morris", "libraries/leaflet", "libraries/rickshaw"]}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---


## Introduction
Compiled US sensus data of all 50 states grouped by divisions to ease comparison of data
<img src="assets/img/AAGRegionalDivisions.jpg" style="margin-top:0px;margin-left:110px;"/>


--- .class #id 

## Comparing Data
Data collected duing a US census in 1977.
  - Population data
  - State area
  - Murder Rate
  - Illiteracy Rate
  - High School Graduation Rate
  - Income
  - Frost
  - Life Expectancy
  

---
## Zoom into divisions
<p>Compare specific statistics based on State division</p>


<div id = 'chart1' class = 'rChart nvd3'></div>
<script type='text/javascript'>
 $(document).ready(function(){
      drawchart1()
    });
    function drawchart1(){  
      var opts = {
 "dom": "chart1",
"width":    800,
"height":    400,
"x": "state.division",
"y": "Murder",
"group": "state.division",
"type": "multiBarChart",
"id": "chart1" 
},
        data = [
 {
 "Population":           3615,
"Income":           3624,
"Illiteracy":            2.1,
"Life.Exp":          69.05,
"Murder":           15.1,
"HS.Grad":           41.3,
"Frost":             20,
"Area":          50708,
"state.division": "East South Central",
"state.abb": "AL" 
},
{
 "Population":            365,
"Income":           6315,
"Illiteracy":            1.5,
"Life.Exp":          69.31,
"Murder":           11.3,
"HS.Grad":           66.7,
"Frost":            152,
"Area":         566432,
"state.division": "Pacific",
"state.abb": "AK" 
},
{
 "Population":           2212,
"Income":           4530,
"Illiteracy":            1.8,
"Life.Exp":          70.55,
"Murder":            7.8,
"HS.Grad":           58.1,
"Frost":             15,
"Area":         113417,
"state.division": "Mountain",
"state.abb": "AZ" 
},
{
 "Population":           2110,
"Income":           3378,
"Illiteracy":            1.9,
"Life.Exp":          70.66,
"Murder":           10.1,
"HS.Grad":           39.9,
"Frost":             65,
"Area":          51945,
"state.division": "West South Central",
"state.abb": "AR" 
},
{
 "Population":          21198,
"Income":           5114,
"Illiteracy":            1.1,
"Life.Exp":          71.71,
"Murder":           10.3,
"HS.Grad":           62.6,
"Frost":             20,
"Area":         156361,
"state.division": "Pacific",
"state.abb": "CA" 
},
{
 "Population":           2541,
"Income":           4884,
"Illiteracy":            0.7,
"Life.Exp":          72.06,
"Murder":            6.8,
"HS.Grad":           63.9,
"Frost":            166,
"Area":         103766,
"state.division": "Mountain",
"state.abb": "CO" 
},
{
 "Population":           3100,
"Income":           5348,
"Illiteracy":            1.1,
"Life.Exp":          72.48,
"Murder":            3.1,
"HS.Grad":             56,
"Frost":            139,
"Area":           4862,
"state.division": "New England",
"state.abb": "CT" 
},
{
 "Population":            579,
"Income":           4809,
"Illiteracy":            0.9,
"Life.Exp":          70.06,
"Murder":            6.2,
"HS.Grad":           54.6,
"Frost":            103,
"Area":           1982,
"state.division": "South Atlantic",
"state.abb": "DE" 
},
{
 "Population":           8277,
"Income":           4815,
"Illiteracy":            1.3,
"Life.Exp":          70.66,
"Murder":           10.7,
"HS.Grad":           52.6,
"Frost":             11,
"Area":          54090,
"state.division": "South Atlantic",
"state.abb": "FL" 
},
{
 "Population":           4931,
"Income":           4091,
"Illiteracy":              2,
"Life.Exp":          68.54,
"Murder":           13.9,
"HS.Grad":           40.6,
"Frost":             60,
"Area":          58073,
"state.division": "South Atlantic",
"state.abb": "GA" 
},
{
 "Population":            868,
"Income":           4963,
"Illiteracy":            1.9,
"Life.Exp":           73.6,
"Murder":            6.2,
"HS.Grad":           61.9,
"Frost":              0,
"Area":           6425,
"state.division": "Pacific",
"state.abb": "HI" 
},
{
 "Population":            813,
"Income":           4119,
"Illiteracy":            0.6,
"Life.Exp":          71.87,
"Murder":            5.3,
"HS.Grad":           59.5,
"Frost":            126,
"Area":          82677,
"state.division": "Mountain",
"state.abb": "ID" 
},
{
 "Population":          11197,
"Income":           5107,
"Illiteracy":            0.9,
"Life.Exp":          70.14,
"Murder":           10.3,
"HS.Grad":           52.6,
"Frost":            127,
"Area":          55748,
"state.division": "East North Central",
"state.abb": "IL" 
},
{
 "Population":           5313,
"Income":           4458,
"Illiteracy":            0.7,
"Life.Exp":          70.88,
"Murder":            7.1,
"HS.Grad":           52.9,
"Frost":            122,
"Area":          36097,
"state.division": "East North Central",
"state.abb": "IN" 
},
{
 "Population":           2861,
"Income":           4628,
"Illiteracy":            0.5,
"Life.Exp":          72.56,
"Murder":            2.3,
"HS.Grad":             59,
"Frost":            140,
"Area":          55941,
"state.division": "West North Central",
"state.abb": "IA" 
},
{
 "Population":           2280,
"Income":           4669,
"Illiteracy":            0.6,
"Life.Exp":          72.58,
"Murder":            4.5,
"HS.Grad":           59.9,
"Frost":            114,
"Area":          81787,
"state.division": "West North Central",
"state.abb": "KS" 
},
{
 "Population":           3387,
"Income":           3712,
"Illiteracy":            1.6,
"Life.Exp":           70.1,
"Murder":           10.6,
"HS.Grad":           38.5,
"Frost":             95,
"Area":          39650,
"state.division": "East South Central",
"state.abb": "KY" 
},
{
 "Population":           3806,
"Income":           3545,
"Illiteracy":            2.8,
"Life.Exp":          68.76,
"Murder":           13.2,
"HS.Grad":           42.2,
"Frost":             12,
"Area":          44930,
"state.division": "West South Central",
"state.abb": "LA" 
},
{
 "Population":           1058,
"Income":           3694,
"Illiteracy":            0.7,
"Life.Exp":          70.39,
"Murder":            2.7,
"HS.Grad":           54.7,
"Frost":            161,
"Area":          30920,
"state.division": "New England",
"state.abb": "ME" 
},
{
 "Population":           4122,
"Income":           5299,
"Illiteracy":            0.9,
"Life.Exp":          70.22,
"Murder":            8.5,
"HS.Grad":           52.3,
"Frost":            101,
"Area":           9891,
"state.division": "South Atlantic",
"state.abb": "MD" 
},
{
 "Population":           5814,
"Income":           4755,
"Illiteracy":            1.1,
"Life.Exp":          71.83,
"Murder":            3.3,
"HS.Grad":           58.5,
"Frost":            103,
"Area":           7826,
"state.division": "New England",
"state.abb": "MA" 
},
{
 "Population":           9111,
"Income":           4751,
"Illiteracy":            0.9,
"Life.Exp":          70.63,
"Murder":           11.1,
"HS.Grad":           52.8,
"Frost":            125,
"Area":          56817,
"state.division": "East North Central",
"state.abb": "MI" 
},
{
 "Population":           3921,
"Income":           4675,
"Illiteracy":            0.6,
"Life.Exp":          72.96,
"Murder":            2.3,
"HS.Grad":           57.6,
"Frost":            160,
"Area":          79289,
"state.division": "West North Central",
"state.abb": "MN" 
},
{
 "Population":           2341,
"Income":           3098,
"Illiteracy":            2.4,
"Life.Exp":          68.09,
"Murder":           12.5,
"HS.Grad":             41,
"Frost":             50,
"Area":          47296,
"state.division": "East South Central",
"state.abb": "MS" 
},
{
 "Population":           4767,
"Income":           4254,
"Illiteracy":            0.8,
"Life.Exp":          70.69,
"Murder":            9.3,
"HS.Grad":           48.8,
"Frost":            108,
"Area":          68995,
"state.division": "West North Central",
"state.abb": "MO" 
},
{
 "Population":            746,
"Income":           4347,
"Illiteracy":            0.6,
"Life.Exp":          70.56,
"Murder":              5,
"HS.Grad":           59.2,
"Frost":            155,
"Area":         145587,
"state.division": "Mountain",
"state.abb": "MT" 
},
{
 "Population":           1544,
"Income":           4508,
"Illiteracy":            0.6,
"Life.Exp":           72.6,
"Murder":            2.9,
"HS.Grad":           59.3,
"Frost":            139,
"Area":          76483,
"state.division": "West North Central",
"state.abb": "NE" 
},
{
 "Population":            590,
"Income":           5149,
"Illiteracy":            0.5,
"Life.Exp":          69.03,
"Murder":           11.5,
"HS.Grad":           65.2,
"Frost":            188,
"Area":         109889,
"state.division": "Mountain",
"state.abb": "NV" 
},
{
 "Population":            812,
"Income":           4281,
"Illiteracy":            0.7,
"Life.Exp":          71.23,
"Murder":            3.3,
"HS.Grad":           57.6,
"Frost":            174,
"Area":           9027,
"state.division": "New England",
"state.abb": "NH" 
},
{
 "Population":           7333,
"Income":           5237,
"Illiteracy":            1.1,
"Life.Exp":          70.93,
"Murder":            5.2,
"HS.Grad":           52.5,
"Frost":            115,
"Area":           7521,
"state.division": "Middle Atlantic",
"state.abb": "NJ" 
},
{
 "Population":           1144,
"Income":           3601,
"Illiteracy":            2.2,
"Life.Exp":          70.32,
"Murder":            9.7,
"HS.Grad":           55.2,
"Frost":            120,
"Area":         121412,
"state.division": "Mountain",
"state.abb": "NM" 
},
{
 "Population":          18076,
"Income":           4903,
"Illiteracy":            1.4,
"Life.Exp":          70.55,
"Murder":           10.9,
"HS.Grad":           52.7,
"Frost":             82,
"Area":          47831,
"state.division": "Middle Atlantic",
"state.abb": "NY" 
},
{
 "Population":           5441,
"Income":           3875,
"Illiteracy":            1.8,
"Life.Exp":          69.21,
"Murder":           11.1,
"HS.Grad":           38.5,
"Frost":             80,
"Area":          48798,
"state.division": "South Atlantic",
"state.abb": "NC" 
},
{
 "Population":            637,
"Income":           5087,
"Illiteracy":            0.8,
"Life.Exp":          72.78,
"Murder":            1.4,
"HS.Grad":           50.3,
"Frost":            186,
"Area":          69273,
"state.division": "West North Central",
"state.abb": "ND" 
},
{
 "Population":          10735,
"Income":           4561,
"Illiteracy":            0.8,
"Life.Exp":          70.82,
"Murder":            7.4,
"HS.Grad":           53.2,
"Frost":            124,
"Area":          40975,
"state.division": "East North Central",
"state.abb": "OH" 
},
{
 "Population":           2715,
"Income":           3983,
"Illiteracy":            1.1,
"Life.Exp":          71.42,
"Murder":            6.4,
"HS.Grad":           51.6,
"Frost":             82,
"Area":          68782,
"state.division": "West South Central",
"state.abb": "OK" 
},
{
 "Population":           2284,
"Income":           4660,
"Illiteracy":            0.6,
"Life.Exp":          72.13,
"Murder":            4.2,
"HS.Grad":             60,
"Frost":             44,
"Area":          96184,
"state.division": "Pacific",
"state.abb": "OR" 
},
{
 "Population":          11860,
"Income":           4449,
"Illiteracy":              1,
"Life.Exp":          70.43,
"Murder":            6.1,
"HS.Grad":           50.2,
"Frost":            126,
"Area":          44966,
"state.division": "Middle Atlantic",
"state.abb": "PA" 
},
{
 "Population":            931,
"Income":           4558,
"Illiteracy":            1.3,
"Life.Exp":           71.9,
"Murder":            2.4,
"HS.Grad":           46.4,
"Frost":            127,
"Area":           1049,
"state.division": "New England",
"state.abb": "RI" 
},
{
 "Population":           2816,
"Income":           3635,
"Illiteracy":            2.3,
"Life.Exp":          67.96,
"Murder":           11.6,
"HS.Grad":           37.8,
"Frost":             65,
"Area":          30225,
"state.division": "South Atlantic",
"state.abb": "SC" 
},
{
 "Population":            681,
"Income":           4167,
"Illiteracy":            0.5,
"Life.Exp":          72.08,
"Murder":            1.7,
"HS.Grad":           53.3,
"Frost":            172,
"Area":          75955,
"state.division": "West North Central",
"state.abb": "SD" 
},
{
 "Population":           4173,
"Income":           3821,
"Illiteracy":            1.7,
"Life.Exp":          70.11,
"Murder":             11,
"HS.Grad":           41.8,
"Frost":             70,
"Area":          41328,
"state.division": "East South Central",
"state.abb": "TN" 
},
{
 "Population":          12237,
"Income":           4188,
"Illiteracy":            2.2,
"Life.Exp":           70.9,
"Murder":           12.2,
"HS.Grad":           47.4,
"Frost":             35,
"Area":         262134,
"state.division": "West South Central",
"state.abb": "TX" 
},
{
 "Population":           1203,
"Income":           4022,
"Illiteracy":            0.6,
"Life.Exp":           72.9,
"Murder":            4.5,
"HS.Grad":           67.3,
"Frost":            137,
"Area":          82096,
"state.division": "Mountain",
"state.abb": "UT" 
},
{
 "Population":            472,
"Income":           3907,
"Illiteracy":            0.6,
"Life.Exp":          71.64,
"Murder":            5.5,
"HS.Grad":           57.1,
"Frost":            168,
"Area":           9267,
"state.division": "New England",
"state.abb": "VT" 
},
{
 "Population":           4981,
"Income":           4701,
"Illiteracy":            1.4,
"Life.Exp":          70.08,
"Murder":            9.5,
"HS.Grad":           47.8,
"Frost":             85,
"Area":          39780,
"state.division": "South Atlantic",
"state.abb": "VA" 
},
{
 "Population":           3559,
"Income":           4864,
"Illiteracy":            0.6,
"Life.Exp":          71.72,
"Murder":            4.3,
"HS.Grad":           63.5,
"Frost":             32,
"Area":          66570,
"state.division": "Pacific",
"state.abb": "WA" 
},
{
 "Population":           1799,
"Income":           3617,
"Illiteracy":            1.4,
"Life.Exp":          69.48,
"Murder":            6.7,
"HS.Grad":           41.6,
"Frost":            100,
"Area":          24070,
"state.division": "South Atlantic",
"state.abb": "WV" 
},
{
 "Population":           4589,
"Income":           4468,
"Illiteracy":            0.7,
"Life.Exp":          72.48,
"Murder":              3,
"HS.Grad":           54.5,
"Frost":            149,
"Area":          54464,
"state.division": "East North Central",
"state.abb": "WI" 
},
{
 "Population":            376,
"Income":           4566,
"Illiteracy":            0.6,
"Life.Exp":          70.29,
"Murder":            6.9,
"HS.Grad":           62.9,
"Frost":            173,
"Area":          97203,
"state.division": "Mountain",
"state.abb": "WY" 
} 
]
  
      if(!(opts.type==="pieChart" || opts.type==="sparklinePlus" || opts.type==="bulletChart")) {
        var data = d3.nest()
          .key(function(d){
            //return opts.group === undefined ? 'main' : d[opts.group]
            //instead of main would think a better default is opts.x
            return opts.group === undefined ? opts.y : d[opts.group];
          })
          .entries(data);
      }
      
      if (opts.disabled != undefined){
        data.map(function(d, i){
          d.disabled = opts.disabled[i]
        })
      }
      
      nv.addGraph(function() {
        var chart = nv.models[opts.type]()
          .width(opts.width)
          .height(opts.height)
          
        if (opts.type != "bulletChart"){
          chart
            .x(function(d) { return d[opts.x] })
            .y(function(d) { return d[opts.y] })
        }
          
         
        
          
        

        
        
        
      
       d3.select("#" + opts.id)
        .append('svg')
        .datum(data)
        .transition().duration(500)
        .call(chart);

       nv.utils.windowResize(chart.update);
       return chart;
      });
    };
</script>

Figure: Murder rate of all states grouped by state division

--- .class #id 

## Customize views
<p>Select division and statistic to update the chart interactively</p>
  - Quick interactive access to relevant data
  - Easy comparison ability
  - Quick access to information

--- .class #id 

## Questions?
<img src="assets/img/ask-the-right-questions.jpg" style="width: 650px;margin-left: 300px;margin-top: 14px;"/>

