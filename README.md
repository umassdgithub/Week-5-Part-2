# Week-5 
## D3 Generators
In these example D3JS Generators are used to create stacked barchart, and area charts.




<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt;">&nbsp;</span></p>
<table cellpadding="0" cellspacing="0" border="0" class="MsoTableGrid" style="width: 708px; border-collapse: collapse; border: none;">
<tbody>
<tr>
<td valign="top" style="width: 110.4pt; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">Generate SVG</span></p>
</td>
<td style="width: 24.6pt; background: #D0CECE; padding: 0in 5.4pt 0in 5.4pt;">
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">1</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">2</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">3</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">4</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">5</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">6</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">7</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">8</span></p>
</td>
<td valign="top" style="width: 5.5in; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">// A simple line chart</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="position: relative; z-index: 251659264;"><span style="position: absolute; left: 32px; top: -22px; width: 3px; height: 60px;"></span></span><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const width &nbsp;&nbsp;= &nbsp;<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>;</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="position: relative; z-index: 251660288;"><span style="position: absolute; left: 38px; top: -29px; width: 25px; height: 71px;"></span></span><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const height &nbsp;= &nbsp;<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>;</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const margin = {top: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, left: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, right: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, bottom: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>}</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const svg = d3.select("body")</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .append("svg")</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .attr("width", width)</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .attr("height", height)</span></p>
</td>
</tr>
<tr>
<td valign="top" style="width: 110.4pt; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">Define data</span></p>
</td>
<td style="width: 24.6pt; background: #D5DCE4; padding: 0in 5.4pt 0in 5.4pt;">
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">10</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">12</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">13</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">14</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">15</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">16</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">17</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">18</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">19</span></p>
</td>
<td valign="top" style="width: 5.5in; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">// Generate data</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const data = [</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="position: relative; z-index: 251661312;"><span style="position: absolute; left: 6px; top: -56px; width: 11px; height: 119px;"></span></span><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {x: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, y:<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>},</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {x: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, y:<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>},</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {x: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, y:<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>},</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {x: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, y:<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>},</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {x: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, y:<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>},</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {x: <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>, y:<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>}];</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;</span></p>
</td>
</tr>
<tr>
<td valign="top" style="width: 110.4pt; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">Define scales</span></p>
</td>
<td style="width: 24.6pt; background: #D9E2F3; padding: 0in 5.4pt 0in 5.4pt;">
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">20</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">21</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">22</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">23</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">24</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">25</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">26</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">27</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">28</span></p>
</td>
<td valign="top" style="width: 5.5in; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">// Scale the date using d3 scale functions</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="position: relative; z-index: 251663360;"><span style="position: absolute; left: 87px; top: -83px; width: 18px; height: 136px;"></span></span><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const xScale = d3.scalePoint()</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .domain([<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>&nbsp;, <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>&nbsp;, <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>&nbsp;, <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>&nbsp;, <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>&nbsp;, <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>])</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .rangeRound([margin.left,width-margin.right])</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const yScale = d3.scaleLinear()</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .domain([<span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>&nbsp;, <span style="color: black; border: solid windowtext 1.0pt; padding: 0in; background: #E7E6E6;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>])</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .range([height-margin.bottom,margin.top]) </span></p>
</td>
</tr>
<tr>
<td valign="top" style="width: 110.4pt; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">Draw Axes</span></p>
</td>
<td style="width: 24.6pt; background: #FBE4D5; padding: 0in 5.4pt 0in 5.4pt;">
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">29</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">30</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">31</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">32</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">33</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">34</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">35</span></p>
</td>
<td valign="top" style="width: 5.5in; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="position: relative; z-index: 251664384;"><span style="position: absolute; left: -41px; top: -166px; width: 104px; height: 132px;"></span></span><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">// Draw Axes</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const xAxis = svg.append("g")</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .attr("transform",`translate(${0},${height-margin.bottom})`)</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .call(d3.axisBottom().scale(xScale))</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const yAxis = svg.append("g")</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .attr("transform",`translate(${margin.left},${0})`)</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .call(d3.axisLeft().scale(yScale))</span></p>
</td>
</tr>
<tr>
<td valign="top" style="width: 110.4pt; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">Line Generator</span></p>
</td>
<td style="width: 24.6pt; background: #FFF2CC; padding: 0in 5.4pt 0in 5.4pt;">
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">36</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">37</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">38</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">39</span></p>
</td>
<td valign="top" style="width: 5.5in; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">// Use line generator to make path element attributes (d)</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const lineGen = d3.line()</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .x(d=&gt;xScale(d.x))</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .y(d=&gt;yScale(d.y))</span></p>
</td>
</tr>
<tr>
<td valign="top" style="width: 110.4pt; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">Bind/Draw data</span></p>
</td>
<td style="width: 24.6pt; background: #E2EFD9; padding: 0in 5.4pt 0in 5.4pt;">
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">40</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">41</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">42</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">43</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">44</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">45</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">46</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">47</span></p>
<p style="text-align: center; margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif; color: #aeaaaa;">48</span></p>
</td>
<td valign="top" style="width: 5.5in; padding: 0in 5.4pt 0in 5.4pt;">
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">// Bind data, and add path element with attributes</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp; const lineChart = svg.selectAll('.Line')</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .data([data])</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .enter()</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .append("path")</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .attr("d",d=&gt;lineGen(d))</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .attr("fill","none")</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .attr("stroke","steelblue")</span></p>
<p style="margin: 0in; font-size: 12pt; font-family: Calibri, sans-serif;"><span style="font-size: 10.0pt; font-family: 'DEJAVU SANS', sans-serif;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .attr("stroke-width",2)</span></p>
</td>
</tr>
</tbody>
</table>
