# Overview

This test suite is based on the following OGC specifications, best practices,
and discussion papers:

  * _Sensor Planning Service Implementation Specification_, version 2.0.0 [OGC 09-000](http://portal.opengeospatial.org/files/?artifact_id=38478)
  * _OpenGIS Web Services Common Specification_, version 1.1.0 [OGC 06-121r3](https://portal.opengeospatial.org/files/?artifact_id=20040)
  * _A URN Namespace for the Open Geospatial Consortium (OGC)_, version 2 [OGC 06-166](https://portal.opengeospatial.org/files/?artifact_id=18747)
  * _Definition Identifier URNs in OGC Namespace_, version 1.1.2 [OGC 07-092r1](https://portal.opengeospatial.org/files/?artifact_id=24045)

## What is tested

  * **Basic/Core conformance class (mandatory operations)**

    * GetCapabilities, GET method/POST method
    * DescribeTasking, POST method
    * Submit, POST method
    * GetStatus, POST method
    * GetTask, POST method
    * DescribeResultAccess, POST method
    * DescribeSensor, POST method
    * This includes testing:
      * All required aspects of the mandatory operations of the SPS: GetCapabilities, DescribeTasking, Submit, GetStatus, GetTask, DescribeResultAccess and DescribeSensor
      * Valid exception reporting according to the specification
      * Conformance Class - State Logger:GetStatus
      * The Capabilities document lists all of the mandatory operations of the SPS specification in the OperationsMetadata section
      * Any non-mandatory operations listed in the OperationsMetadata section have valid SPS operation names

## What is not tested

Optional operations of the SPS:

  * ReservationManager interface: Reserve, Confirm 
  * FeasibilityController interface: GetFeasibility
  * TaskUpdater interface: Update
  * TaskCanceller interface: Cancel
  * SensorDescriptionManager interface: UpdateSensorDescription

## Test data

This test suite does not require test data. The compliance tests were designed
to be generic enough to work with any SPS implementation providing access to
any sensor system.

## Namespaces
  * SensorML v1.0.0 - http://www.opengis.net/sensorML/1.0
  * SensorML v1.0.1 - http://www.opengis.net/sensorML/1.0.1
  * TML - http://www.opengis.net/tml
  * SWE Common - http://www.opengis.net/swe/1.0
  * OWS Common - http://www.opengis.net/ows
  * SPS - http;//www.opengis.net/sps/2.0
  * GML - http://www.opengis.net/gml

## Schemas

All schemas used in these tests are located in the OGC schema repository:
<http://schemas.opengis.net>.

## Release Notes
Release notes are available from the [relnotes.html](relnotes.html).
