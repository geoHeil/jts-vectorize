# vectorizaton of images in java

```
java.lang.IllegalArgumentException: RangeLookup: No OperationDescriptor is registered in the current operation registry under this name.
	at javax.media.jai.JAI.createNS(JAI.java:1070)
	at javax.media.jai.JAI.create(JAI.java:973)
	at org.geotools.image.ImageWorker.rangeLookup(ImageWorker.java:5016)
	at org.geotools.process.raster.RangeLookupProcess.execute(RangeLookupProcess.java:188)
	at org.geotools.process.raster.RangeLookupProcess.execute(RangeLookupProcess.java:234)
	at org.geotools.process.raster.PolygonExtractionProcess.execute(PolygonExtractionProcess.java:167)
	at FooJava.getWktForDbRangeFromRaster(FooJava.java:57)
	at FooJava.main(FooJava.java:36)
```



when looking at the jai registration files in [registryFilesGenerated](registryFilesGenerated) none of them sadly contains the `vectors` registration.

When executing using IntelliJ

it works just fine
````
POLYGON ((0 0, 50 0, 50 50, 150 50, 150 150, 200 150, 200 250, 50 250, 50 200, 100 200, 100 150, 0 150, 0 0))

````
