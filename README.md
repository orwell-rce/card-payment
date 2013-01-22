#GPS

## Package.
The main Namespace is com.progress.demo.rce.gps

## Events.

* **NewPOI**(string, location). It register a new Point Of Interest with its name (the string) and its location .

* **Position**(integer, location). It represents the position of the client (the integer is the client id) and its location.

* **NewSim**(integer, float, float). It starts the internal gps-simulator. The integer represents the client Id, the first float represents the maximum allowed value of the X-axis and the second float represents the maximum allowed value in the Y-axis.

* **AlertPOI**(NewPOI, integer, Position). It alerts about the POI, with its id integer and the client position.


