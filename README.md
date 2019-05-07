# ![LOGO](logo.png) AviationData.Systems Airports API V1 **flow**ground Connector

## Description

A generated **flow**ground connector for the AviationData.Systems Airports API V1 API (version v1).

Generated from: https://api.apis.guru/v2/specs/aviationdata.systems/v1/swagger.json<br/>
Generated at: 2019-05-07T17:37:04+03:00

## API Description



## Authorization

Supported authorization schemes:
- Basic Authentication

## Actions

### Autocomplete airport names. Returns a maximum of 10 airport names.

> Required parameters: airport_name, airport_service_type. Optional parameter: country code (ISO 3166-1).

*Tags:* `AutoCompleteAirportName`

#### Input Parameters
* `airport_name` - _required_ - Required: The airports name
* `airport_service_type` - _required_ - Required: Needs to be: All, Scheduled or NonScheduled
    Possible values: All, Scheduled, NonScheduled.
* `optional_country_code` - _optional_ - Optional: Country code (ISO 3166-1). This can be found via /countries

### Search for airport by IATA code

> Required parameters: airport_iata

*Tags:* `AirportIATA`

#### Input Parameters
* `airport_iata` - _required_ - Required: The airports IATA code

### Search for airport by name

> Required parameters: airport_name, api_mode

*Tags:* `AirportDetails`

#### Input Parameters
* `airport_name` - _required_ - Required: The airports name

### Search for airports by location

> Required parameters: result_count, latitude, longitude, airport_service_type

*Tags:* `NearestAirports`

#### Input Parameters
* `result_count` - _required_ - Required: Number of airports to return. Min: 1 Max: 20
* `latitude` - _required_ - Required: Latitude
* `longitude` - _required_ - Required: Longitude

### Country airports. Returns a list of airports for a country code(ISO 3166-1 alpha-2 code)

> Required parameters: country code (ISO 3166-1), airport_service_type.

*Tags:* `CountryAirportList`

#### Input Parameters
* `country_code` - _required_ - Country code (ISO 3166-1). This can be found via /countries
* `airport_service_type` - _required_ - Required: Needs to be: All, Scheduled or NonScheduled
    Possible values: All, Scheduled, NonScheduled.

### Country list. Returns a list of countries where airport data is available

*Tags:* `CountryList`

## License

**flow**ground :- Telekom iPaaS / aviationdata-systems-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
