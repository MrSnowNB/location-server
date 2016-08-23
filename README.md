# location-server
Return state from lat/long using point-in-polygon

## Objective

What we need is a server to tell us which state, if any, a point is in.
Some simplified geometries are included in states.json (so greatly simplified,
that some of the smaller ones disappear).


## Dependencies

Python 3


## Run Instructions

You can either run state-server from the command line:

  $ ./state-server &
  [1] 21507
  $ curl  -d "longitude=-77.036133&latitude=40.513799" http://localhost:8080/
  ["Pennsylvania"]
  $
  
or you can start it from the command line:

  $ ./state-server
  
and test it through using a browser GUI by opening http://localhost:8080/ in a web browser.
