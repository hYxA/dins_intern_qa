# Тестовое задание **Intern QA**

## Текст задания

1. Create a free account at weatherbit.io and get your API Key. Wait for 20 minutes until it will be activated.
1. Open the swagger specification from [the attached file](/raw.txt) in any swagger editor. Try to execute these requests in the editor with your API Key and different parameters.
1. Write check list for testing of this API. You report should look like check list with examples of requests (curl or postman collection). Also write detailed test-cases for any 3 checks.
1. Try to find some bugs in the API.

## Первый запуск
### Steps 

1. Open the swagger specification in POSTMAN
1. Substitute the values key, units, lat, lon
1. Send request

### Expected result

Get observations

### Actual result

{ 
    "error": "Invalid Parameters supplied."
}

### Comments

Values lat and lon is Query params, not a path.


## Check list

1. Enter params without lat/lon
 
    { lang:en
    units:m
    state_code:771
    //lat:59.95
    //lon:30.32
    key:ddf5b7e63db6408bbfe9e102a0f8bb21	}