ebongo_notifier
===============

Know where your bus is at a glance.

===============

Formats
###
The Bongo API can be retrieved in a number of different formats. These are XML, JSON and JSONP. The default format is XML, so if you do not pass a format parameter, you will receive XML back. To get JSON or JSONP, pass the format parameter in the URL. For example, if you wanted to get the route list in JSON, you would enter

http://api.ebongo.org/routelist?format=json&api_key=XXXX

####

Route Listing
####
This will display a list of all routes in the Bongo system.
URI - http://api.ebongo.org/routelist?api_key=XXXX
#####
Route Info
####
This will display information for a specific route. This takes two parameters,**_agency_** for the transit agency for the route and **_route_** for the route tag.
URI - http://api.ebongo.org/route?agency=XXXX&route=XXXX&api_key=XXXX
#####
Stop Listing
####
This will display all stops in Bongo. Note, this may take some time to load due to the amount of information retrieved.
URI - http://api.ebongo.org/stoplist?api_key=XXXX
#####
Stop Info
####
This will display information for a specific stop. This takes one parameter, **_stopid_** for stop number
URI - http://api.ebongo.org/stop?stopid=XXXX&api_key=XXXX
#####
Predictions
####
This will display arrival predictions for a specific stop. This takes one parameter, **_stopid_** for stop number
URI - http://api.ebongo.org/prediction?stopid=XXXX&api_key=XXXX
#####
Bus Locations
####
This will display location information for buses on a specific route. This takes two parameters, **_agency_** for the transit agency for the route and **_route_** for the route tag.
URI - http://api.ebongo.org/buslocation?agency=XXXX&route=XXXX&api_key=XXXX
#####

