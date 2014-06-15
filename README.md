ebongo_notifier
===============

Know where your bus is at a glance.

===============

###Formats
The Bongo API can be retrieved in a number of different formats. These are XML, JSON and JSONP. The default format is XML, so if you do not pass a format parameter, you will receive XML back. To get JSON or JSONP, pass the format parameter in the URL. For example, if you wanted to get the route list in JSON, you would enter

http://api.ebongo.org/routelist?format=json&api_key=XXXX

######Returns
```Ruby
{	"routes" => [
			        	{ "route" => {
														"name"=>"", 
														"tag"=>"", 
														"agency"=>""}
                 }
              ]
}
```
####Route Listing
This will display a list of all routes in the Bongo system.
URI - http://api.ebongo.org/routelist?format=json&api_key=XXXX

####Route Info
This will display information for a specific route. This takes two parameters,**_agency_** for the transit agency for the route and **_route_** for the route tag.
URI - http://api.ebongo.org/route?agency=XXXX&route=XXXX&format=json&api_key=XXXX

####Stop Listing
This will display all stops in Bongo. Note, this may take some time to load due to the amount of information retrieved.
URI - http://api.ebongo.org/stoplist?format=json&api_key=XXXX

####Stop Info
This will display information for a specific stop. This takes one parameter, **_stopid_** for stop number
URI - http://api.ebongo.org/stop?stopid=XXXX&format=json&api_key=XXXX

####Predictions
This will display arrival predictions for a specific stop. This takes one parameter, **_stopid_** for stop number
URI - http://api.ebongo.org/prediction?stopid=XXXX&format=json&api_key=XXXX

####Bus Locations
This will display location information for buses on a specific route. This takes two parameters, **_agency_** for the transit agency for the route and **_route_** for the route tag.
URI - http://api.ebongo.org/buslocation?agency=XXXX&route=XXXX&format=json&api_key=XXXX

###DATA

| Agencies |
|:------:|
| coralville |
| iowa-city |
| uiowa |

| Route | Tag | Agency|
|:-----:|:---:|:-----:|
|10th Street|10thst|coralville|
|AM Express|amexpress|coralville|
|AM North Liberty|amnorthlib|coralville|
|Lantern Park|lantern|coralville|
|Night/Saturday|nightsat|coralville|
|PM Express|pmexpress|coralville|
|PM North Liberty|pmnorthlib|coralville|
|PM Special|pmspecial|coralville|
|7th Avenue|7thave|iowa-city|
|Broadway|brdwy|iowa-city|
|Broadway Night & Weekend|brdwynw|iowa-city|
|Court Hill|courthill|iowa-city|
|Cross Park|crosspark|iowa-city|
|Eastside Express|eastex|iowa-city|
|Eastside Loop AM|esla|iowa-city|
|Eastside Loop PM|eslp|iowa-city|
|Event Shuttle|eventshuttle|iowa-city|
|Free Shuttle North|shuttlen|iowa-city|
|Free Shuttle South|shuttles|iowa-city|
|Lakeside|lakeside|iowa-city|
|Mall|mall|iowa-city|
|Manville Heights|manville|iowa-city|
|Manville Heights Night & Weekend|manvillenw|iowa-city|
|Melrose Express|melrose|iowa-city|
|North Dodge|ndodge|iowa-city|
|North Dodge Night & Weekend|ndodgenw|iowa-city|
|Oakcrest|oakcrst|iowa-city|
|Oakcrest Night & Weekend|oakcrstnw|iowa-city|
|Plaen View|plaenview|iowa-city|
|Rochester|rochester|iowa-city|
|Towncrest|towncrst|iowa-city|
|Towncrest Night & Weekend|towncrstnw|iowa-city|
|Westport|westport|iowa-city|
|Westside Hospital|westhosp|iowa-city|
|Westwinds|westwinds|iowa-city|
|Westwinds Night & Weekend|westwindsnw|iowa-city|
|ABW/Studio Arts|abwstart|uiowa|
|Blue|blue|uiowa|
|East Campus Shuttle|ecs|uiowa|
|Finals Week Interdorm|interdormfnls|uiowa|
|Hawk Express|hawkexpress|uiowa|
|Hawk Lot/Hospital|hawklot|uiowa|
|Hawkeye Hospital|hawkhosp|uiowa|
|Hawkeye Interdorm|hawkdorm|uiowa|
|Hospital|hospital|uiowa|
|Hospital via Hancher|hosphanch|uiowa|
|Hospital/VA Loop|hospva|uiowa|
|Interdorm|interdorm|uiowa|
|Mayflower Shuttle|mayflower|uiowa|
|Music/Theatre Shuttle|mts|uiowa|
|Night Pentacrest|pentnight|uiowa|
|Orientation Shuttle|orientation|uiowa|
|Pentacrest|pentacrest|uiowa|
|Red|red|uiowa|
|Research Park|research|uiowa|
|Studio Arts Shuttle|studart|uiowa|

