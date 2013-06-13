p1lapchart
==========
I've combined my love of code and motorsports together to automatically create 
[lap charts](http://www.collinsdictionary.com/dictionary/english/lap-chart) from html race results posted at
[MyLaps.com](http://mylaps.com).  These charts show cars and their race positions at each lap in the race.

A server runs a [Node](http://nodejs.org) web application that 
[web scrapes](http://en.wikipedia.org/wiki/Web_scraping) the source html at 
[MyLaps.com](http://mylaps.com) (top screenshot) using [jQuery](http://jquery.org).
It produces a JSON representation of the race information.

The final graphical visualizations (bottom screenshot) are created on the browser with code that uses
[D3](http://d3js.org/) to graphically render the race information from the JSON objects.  

<table>
<tr><td align="center">
<a href="http://www.mylaps.com/en/lapchart/2695656"><img src="https://github.com/kenklin/p1lapchart/blob/master/images/p1lapchart-mylaps.png?raw=true"></a>
<br><i>Source html from mylaps.com
</td></tr>
<tr><td align="center">
&#8595;
<br><a href="https://github.com/kenklin/p1lapchart/blob/master/node-p1lapchart.js"><strong>node_p1lapchart.js</strong></a>
<br><i>jQuery web scraper implemented as Node application
<br>&#8595;
</td></tr>
<tr><td align="center">
<a href="https://github.com/kenklin/p1lapchart/blob/master/lapchart/2695656.json">2695656.json</a>
<br><i>Resulting JSON object
</td></tr>
<tr><td align="center">
&#8595;
<br><a href="https://github.com/kenklin/p1lapchart/blob/master/index.html"><strong>index.html</strong></a>
<br><i>D3 visualization
<br>&#8595;
</td></tr>
<tr><td align="center">
<a href="http://kenlin.com/x/p1lapchart/"><img src="https://github.com/kenklin/p1lapchart/blob/master/images/p1lapchart-d3.png?raw=true"></a>
</td></tr>
</table>
