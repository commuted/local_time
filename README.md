# local_time
From geo coordinates return local time using timezone and daylight savings time.

Uses local tables for embedding in a device without connectivity which has access to geo coordinates, such as GPS/GLONAS/GALILEO.

valid range 1900 - 2250

Usage:

npm --install @commuted/local_time, or just npm --install in git repository to get dependancies. 

Create file with these lines with epoch time and location
var what_time = require('@commuted/local_time')
console.log(what_time.get_local_correction(1528616801, 47.650499, -122.350070));

Returns correction in seconds. 
