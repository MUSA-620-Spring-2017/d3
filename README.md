## D3 Examples

[Simple animated circle example](https://bl.ocks.org/galkamax/c19642317ac807fe13a99bbcf2eaaa75) ([code](https://github.com/MUSA-620-Fall-2017/d3/blob/master/circle-example.html))

[Animated NYC taxi pickups over 24 hours](https://bl.ocks.org/galkamax/f3ecfeb0b4ebbbec104e87a08dc4806e) ([code](https://github.com/MUSA-620-Fall-2017/d3/blob/master/nyc-taxi-pickups.html))-- This is the D3 version of the map I showed in class. The code can work for any map. Plug in your own geojson file and make a few modifications.



## D3 Useful Links

[D3 gallery](https://github.com/d3/d3/wiki/Gallery)

[D3 documentation](https://github.com/d3/d3/blob/master/API.md)

[bl.ocks.org](https://bl.ocks.org/-/about) - lots of D3 examples. Search [Gist](https://gist.github.com/) for examples or search in Google using the site: operator ("site:bl.ocks.org").

[Example]



## Simple circle example

<script src="https://d3js.org/d3.v4.min.js"></script>

<svg></svg>
<body>
<script>

var svg = d3.select("svg")
	.style("width","100%")
	.style("height","100%");

svg.append("circle")
	.attr("cx",100)
	.attr("cy",200)
	.style("fill","blue")
	.attr("r",50);
	
	
svg.append("circle")
	.attr("cx",500)
	.attr("cy",200)
	.style("fill","red")
	.attr("r",20);


</script>
</body>
