# Week-5 
## D3 Generators
In these example D3JS Generators are used to create stacked barchart, and area charts.

A Simple Line Chart with D3JS

You will need to import d3js library from d3js.org, and include this code in a script tag in HTML file

 

Generate SVG

	

1

2

3

4

5

6

7

8

	

// A simple line chart

    const width   =           ;

    const height  =           ;

    const margin = {top:       , left:       , right:       , bottom:        }

    const svg = d3.select("body")

        .append("svg")

        .attr("width", width)

        .attr("height", height)




Define data

	

10

12

13

14

15

16

17

18

19

	

// Generate data

    const data = [

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              }];

 




Define scales

	

20

21

22

23

24

25

26

27

28

	

// Scale the date using d3 scale functions

    const xScale = d3.scalePoint()

        .domain([            ,            ,            ,            ,            ,           ])

        .rangeRound([margin.left,width-margin.right])

 

    const yScale = d3.scaleLinear()

        .domain([           ,           ])

        .range([height-margin.bottom,margin.top])




Draw Axes

	

29

30

31

32

33

34

35

	

// Draw Axes

    const xAxis = svg.append("g")

            .attr("transform",`translate(${0},${height-margin.bottom})`)

            .call(d3.axisBottom().scale(xScale))

    const yAxis = svg.append("g")

        .attr("transform",`translate(${margin.left},${0})`)

        .call(d3.axisLeft().scale(yScale))




Line Generator

	

36

37

38

39

	

// Use line generator to make path element attributes (d)

    const lineGen = d3.line()

            .x(d=>xScale(d.x))

            .y(d=>yScale(d.y))




Bind/Draw data

	

40

41

42

43

44

45

46

47

48

	

// Bind data, and add path element with attributes

    const lineChart = svg.selectAll('.Line')

        .data([data])

        .enter()

        .append("path")

        .attr("d",d=>lineGen(d))

        .attr("fill","none")

        .attr("stroke","steelblue")

        .attr("stroke-width",2)

 

 

A Simple Bar Chart with D3JS

You will need to import d3js library from d3js.org, and include this code in a script tag in HTML file

 

Generate SVG

	

1

2

3

4

5

6

7

8

	

// A simple bar chart

    const width   =           ;

    const height  =           ;

    const margin = {top:       , left:       , right:       , bottom:        }

    const svg = d3.select("body")

        .append("svg")

        .attr("width", width)

        .attr("height", height)




Define data

	

10

12

13

14

15

16

17

18

19

	

// Generate data

    const data = [

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              }];

 




Define scales

	

20

21

22

23

24

25

26

27

28

	

// Scale the date using d3 scale functions

    const xScale = d3.scaleBand()

        .domain([            ,            ,            ,            ,            ,           ])

        .rangeRound([margin.left,width-margin.right])

 

    const yScale = d3.scaleLinear()

        .domain([           ,           ])

        .range([height-margin.bottom,margin.top])




Draw Axes

	

29

30

31

32

33

34

35

	

// Draw Axes

    const xAxis = svg.append("g")

            .attr("transform",`translate(${0},${height-margin.bottom})`)

            .call(d3.axisBottom().scale(xScale))

    const yAxis = svg.append("g")

        .attr("transform",`translate(${margin.left},${0})`)

        .call(d3.axisLeft().scale(yScale))




Line Generator

	

36

37

38

39

	

// Use line generator to make path element attributes (d)

    const lineGen = d3.line()

            .x(d=>xScale(d.x))

            .y(d=>yScale(d.y))




Bind/Draw data

	

40

41

42

43

44

45

46

47

48

49

50

51

52

53

	

   

// Bind data, and draw rectangles

    const barWidth = 50;

    const barChart = svg.selectAll('.rects')

        .data(data)

        .enter()

        .append("rect")

        .attr("x",d=>xScale(d.x) + xScale.bandwidth()/2 - barWidth/2)

        .attr("y",d=>yScale(d.y))

        .attr("width",barWidth)

        .attr("height",d=>height-margin.bottom- yScale(d.y))

        .attr("fill","#fefefe")

        .attr("stroke","steelblue")

        .attr("stroke-width",.8)

 

A Simple Scatterplo

 t with D3JS

You will need to import d3js library from d3js.org, and include this code in a script tag in HTML file

 

 

Generate SVG

	

1

2

3

4

5

6

7

8

	

// A simple scatterplot

    const width   =           ;

    const height  =           ;

    const margin = {top:       , left:       , right:       , bottom:        }

    const svg = d3.select("body")

        .append("svg")

        .attr("width", width)

        .attr("height", height)




Define data

	

10

12

13

14

15

16

17

18

19

	

// Generate data

    const data = [

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              },

        {x:               , y:              }];

 




Define scales

	

20

21

22

23

24

25

26

27

28

	

// Scale the date using d3 scale functions

    const xScale = d3.scaleLinear()

        .domain([            ,            ])

        .range([margin.left,width-margin.right])

 

    const yScale = d3.scaleLinear()

        .domain([           ,           ])

        .range([height-margin.bottom,margin.top])




Draw Axes

	

29

30

31

32

33

34

35

	

// Draw Axes

    const xAxis = svg.append("g")

            .attr("transform",`translate(${0},${height-margin.bottom})`)

            .call(d3.axisBottom().scale(xScale))

    const yAxis = svg.append("g")

        .attr("transform",`translate(${margin.left},${0})`)

        .call(d3.axisLeft().scale(yScale))




Bind/Draw data

	

36

37

38

39

40

41

42

43

44

46

47

48

	

 

// Bind data and add Circles to the data points

   const scatterPlot = svg.selectAll('.circles')

        .data(data)

        .enter()

        .append("circle")

        .attr("cx",d=>xScale(d.x))

        .attr("cy",d=>yScale(d.y))

        .attr("r",5)

        .attr("fill","steelblue")

        .attr("stroke","darkblue")

        .attr("stroke-width",.4)

 




 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 




                                                   
