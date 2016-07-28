## Synopsis

Project exposing 3 operations for currency variation calculation, retrieving top 10 popular movies and querying artist and track details.

## Motivation

Test project requeste by ABI as part of resources evaluation to be part of a nem project. 

## Installation

Download anypoint studio project source from:
[https://github.com/bruno-r-ribeiro/abi/tree/master/abitestapi](https://github.com/bruno-r-ribeiro/abi/tree/master/abitestapi)

## API Reference

Below follows the list of operations exposed by this project and their corresponding endpoints

######- Top 10 popular movies: [GET]
[http://localhost:8081/api/popularMovies](http://localhost:8081/api/popularMovies)

######- Query artist and track details: [POST]
[http://localhost:8081/api/queryArtistTrack](http://localhost:8081/api/queryArtistTrack)

######- Calculate value variation: [POST]
[http://localhost:8081/api/valueVariation](http://localhost:8081/api/valueVariation)
  
## Tests

For testing this application, start Anypoint Studio and import the project and run as mulesoft application.
Below follows the parameter/body to be used for testing each operation:

######- Top 10 popular movies:
Get request operation with no parameters

######- Query artist and track details:
Post message with artist(required) and track fields as per below example.
```
{	
"artist": "Cher", 
"track": "believe"
}
```

######- Calculate value variation:
Post message with start-date(required) and end-date(required) fields as per below example.
```
{
  "start-date": "2016-07-01",
  "end-date": "2016-07-21"
}
```
