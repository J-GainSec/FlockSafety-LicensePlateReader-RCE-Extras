# FlockSafety-LicensePlateReader-RCE-Extras
Additional materials for GainSec's Flock Safety Security Research 4th Disclosure in regards to their Sparrow/Falcon License Plate Readers. 

I included the top 100 results from 09/2025 as part of these Repo as well named: [GainSec-FlockSafety-SSID-wigle-responseresponse_1758444525534.json](https://github.com/J-GainSec/FlockSafety-LicensePlateReader-RCE-Extras/blob/main/GainSec-FlockSafety-SSID-wigle-responseresponse_1758444525534.json)

Additionally below is a picture of one result from when GainSec checked.

<img src="https://gainsec.com/wp-content/uploads/2025/09/Wigle-showing-SSIDs.png" alt="Flock Safety LPR Wigle SSIDs" width="600"/>

Read the rest of the write-up HERE (TBP 09/27/25)
And a write-up specific to the wireless RCE HERE (TBP 09/27/25)


## Curl Command to query Wigle for active hotspots

`curl -u "APINAME:APIKEY"   -H "Accept: application/json"   -H "Content-Type: application/x-www-form-urlencoded"   --data "ssid=flock%&freenet=off"   "https://api.wigle.net/api/v2/network/search`