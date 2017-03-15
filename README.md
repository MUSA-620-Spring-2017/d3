# D3 - Useful Links

[D3 gallery](https://github.com/d3/d3/wiki/Gallery)

[D3 documentation](https://github.com/d3/d3/blob/master/API.md)

[bl.ocks.org](https://bl.ocks.org/-/about) - lots of D3 examples. Search [Gist](https://gist.github.com/) for examples or search in Google using the site: operator ("site:bl.ocks.org").


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
