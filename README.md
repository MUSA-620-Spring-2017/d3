## D3 Examples

[Simple transition / click event example](https://bl.ocks.org/galkamax/c19642317ac807fe13a99bbcf2eaaa75) ([code](https://github.com/MUSA-620-Fall-2017/d3/blob/master/circle-example.html)) -- click the bubble to start the transition

[Animated NYC taxi pickups over 24 hours](https://bl.ocks.org/galkamax/f3ecfeb0b4ebbbec104e87a08dc4806e) ([code](https://github.com/MUSA-620-Fall-2017/d3/blob/master/nyc-taxi-pickups.html))-- This is the D3 version of the [3D map I showed in class](https://maps.blueshift.io/nyc-hourly-taxi-pickups?embed=1). The code can work for any map. Plug in your own geojson file and make a few modifications.

## Running D3 (Javascript) locally from your computer

In general, you can use any standard text editor to write Javascript code. You only have to open it with your browser to run the code. For example, to run the [circle-example.html](https://github.com/MUSA-620-Fall-2017/d3/blob/master/circle-example.html) file in this repo, you only have to download it and open it in Chrome.

The only issue with running Javascript locally is when the Javascript needs to load an external file. For example, the animated taxi pickup map needs to load nyctaxipickups.geojson. For security reasons, Javascript cannot load files directly from your hard drive. Here are two ways of getting around this issue.

**Solution 1**: Download a [Javascript IDE](http://ourcodeworld.com/articles/read/200/top-7-best-free-web-development-ide-for-javascript-html-and-css) and run your Javascript code from there.

**Solution 2**: Start up a local server manually
- Save the nyc-taxi-pickups.html and nyctaxipickups.geojson files to the same folder on your computer.
- From the command line, navigate to that directory and enter "python -m SimpleHTTPServer 8000"
- Now you will be able to run the file by typing this into your browser: http://localhost:8000/nyc-taxi-pickups.html

## D3 Useful Links

[D3 gallery](https://github.com/d3/d3/wiki/Gallery)

[D3 documentation](https://github.com/d3/d3/blob/master/API.md)

[bl.ocks.org](https://bl.ocks.org/-/about) - lots of D3 examples. Search [Gist](https://gist.github.com/) for examples or search in Google using the site: operator ("site:bl.ocks.org").



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
