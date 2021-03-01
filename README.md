# Ember Interview Practice

### Weather Ember App

Please build a simple Ember application that runs locally and displays a 5 day weather forecast for a given location "woe id".

You can use https://www.metaweather.com/api/#location or another free weather api if you prefer. You can find more working woe ids here https://www.metaweather.com/map/

### Deliverable Details

- should show a 5 day forecast with date, weather icon, high/low temp and weather description i.e. "snow or light rain"
- should be able to update the woe id with a text field and submit button
- should show loading state when new woe id is submitted
- please add appropriate test coverage

### Deliverables

Please share the project that is runnable locally. Please share via a private github repo by adding @bauerjon as a collaborator.

### Sample Api Requests

- Forecast using woeid: https://www.metaweather.com/api/location/44418/
- Icon for given weather abbreviation: https://www.metaweather.com/static/img/weather/sn.svg

### CORS Gotchas

You will run into `Cross-Origin Request Blocked` errors when trying to access the metaweather api directly from the browser. You can set up a simple proxy server yourself or use something like https://cors-anywhere.herokuapp.com/ to make the request.

For example

```
$.get( "https://cors-anywhere.herokuapp.com/https://www.metaweather.com/api/location/44418/", function( data ) {
  alert( JSON.stringify(data) );
});
```

