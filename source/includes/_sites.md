# Sites

## Get All Sites - App


> The above command returns JSON structured like this:

```json
[
  {
    "coordinates": {
      "lat": 19.076,
      "lng": 72.8992184
    },
    "id": 7987,
    "uuid": "78015610-2022-47a1-94b3-df26903d9201",
    "location": {
      "type": "Point",
      "coordinates": [
        72.8992184,
        19.076
      ]
    },
    "name": "IIT Bombai",
    "siteTypeId": 12,
    "address": "Powai"
  }
]
```
This endpoint retrieves all sites associated with the logged in service provider.

### HTTP Request

`GET /api/sites`

### HTTP Header

`Authorization: <token>`


## Create Site - App

> The above command returns JSON structured like this:

```json

{
  "coordinates": {
    "lat": 19.076,
    "lng": 72.8992184
  },
  "id": 7987,
  "uuid": "78015610-2022-47a1-94b3-df26903d9201",
  "location": {
    "type": "Point",
    "coordinates": [
      72.8992184,
      19.076
    ]
  },
  "name": "IIT Bombai",
  "siteTypeId": 12,
  "address": "Powai"
}
```

This endpoint creates a new site in an unapproved state.

### HTTP Request

`POST /api/sites`

### HTTP Header

`Authorization: <token>`

> Data needs to sent in the format like below:

```json
{
  "name": "Site name",
  "address": "{{address}}",
  "location": {
    "lat": "{{latitude}}"
    "lng": "{{longitude}}"
  }
}

```

> The above command returns JSON structured like this:

```json

{
  "coordinates": {
    "lat": 19.076,
    "lng": 72.8992184
  },
  "id": 7987,
  "uuid": "78015610-2022-47a1-94b3-df26903d9201",
  "location": {
    "type": "Point",
    "coordinates": [
      72.8992184,
      19.076
    ]
  },
  "name": "IIT Bombai",
  "siteTypeId": 12,
  "address": "Powai"
}
```

## Get All Sites - Dashboard

> The above command returns JSON structured like this:

```json
{
  "sites": 
    [
      {
        "coordinates": {
          "lat": 19.076,
          "lng": 72.8992184
        },
        "id": 7987,
        "uuid": "78015610-2022-47a1-94b3-df26903d9201",
        "location": {
          "type": "Point",
          "coordinates": [
            72.8992184,
            19.076
          ]
        },
        "name": "IIT Bombai",
        "siteTypeId": 12,
        "address": "Powai",
        "customerId": 5,
        "cityId": 1333,
        "siteId": "45676543",
        "regionId": 1,
        "pincode": null,
        "approved": true,
        "createdAt": "2017-09-21T19:47:29.901Z",
        "updatedAt": "2017-09-21T19:47:29.901Z"
      }
    ]
  "total_count": 5,
  "page": 1,
  "per_page": 10
}
```
This endpoint retrieves all sites matching the given filters

### HTTP Request

`GET /api/sites`

### HTTP Header

`Authorization: <token>`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
per_page | 10 | No. of items to retreive
page | 0 | Pagination Index
bounds[east] | null | Longitude of right line of bounding box
bounds[west] | null | Longitude of left line of bounding box
bounds[south] | null | Latitude of bottom line of bounding box
bounds[north] | null | Latitude of top line of bounding box

