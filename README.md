#Google Places API - Java

This is just a lightweight wrapper of the Google Places API for Java. Currently only the search action is supported.

##Example Usage
```
GooglePlaces places = new GooglePlaces( "API_KEY" );
PlacesResult result = places.search( 40.10744f, -88.22724f, 5000, PlacesQueryOptions.create( ).keyword( "willard" ), false );
		
System.out.println( result.getStatus( ) );
for ( Place place : result )
	System.out.println( place.getName( ) + " " + place.getGeometry( ).getLocation( ) );
```

##Dependencies
 * [Apache HttpClient 4.2](http://hc.apache.org/)
 * [cg-jcommons](https://github.com/claygregory/cg-jcommons)

##Binary Download
 * [Latest JAR](http://www.claygregory.com/projects/google-places-api-java/releases/0.1-SNAPSHOT/google-places-api-java-0.1-SNAPSHOT.jar)
 * [Latest JAR with dependencies](http://www.claygregory.com/projects/google-places-api-java/releases/0.1-SNAPSHOT/google-places-api-java-0.1-SNAPSHOT-jar-with-dependencies.jar)