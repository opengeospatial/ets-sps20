# SPS 2.0 Test Suite Release Notes

## 1.12 (2025-03-05)

Attention: Java 17 and Tomcat 10.1 are required.

- [#4](https://github.com/opengeospatial/ets-sps20/issues/4): Migrate test suite to TEAM Engine 6 (Java 17)
- [#3](https://github.com/opengeospatial/ets-sps20/issues/3): Deployment to Central Maven Repository fails

## 1.11 (2018-05-18)

- [#1](https://github.com/opengeospatial/ets-sps20/issues/1): Update CTL with better information about conformance classes.

## 1.9 (2015-02-19)

- Cleaned the structure of the test. The test scripts (ctl) have not changed.
- Starting this revision, the revision number will follow the conventions described in the [wiki](https://github.com/opengeospatial/cite/wiki/OGC-Compliance-Testing-Tools)

## r8 (2014/03/06)

- Depended on xlink schemas 1.1 (W3C XLink 1.1) . "http://schemas.opengis.net/xlink/1.0.0/xlinks.xsd" will be changed to "http://www.w3.org/1999/xlink.xsd" and
		"xlink:simpleLink" will be changed to "xlink: simpleAttrs"

## r7

- Cleaned documentation (index.html and relnotes) (20130903) - lb
- Add <li>Conformance Class - State Logger:GetStatus</li> to index.html.

## r6 (2013-05-29)

- Removed redundant assertion checks that duplicate XML Schema constraints
  (DescribeResultAccess-CheckResponse, DescribeResultAccess-ReferenceGroup.1).
- Replaced some nested xsl:choose/xsl:when elements with xsl:if so all constraints 
  are checked (instead of exiting block after first failing assertion).
- Produce warning in DescribeResultAccess-ReferenceGroup.1 if resource reference 
  does not match any known case.


## r5 (2013-03-21)

- removed nested ctl:package elements (intended as document element only)
- SPSETS.xml line:8017 bug fixed.  "or" change to "and"
- config.xml: Added "Beta" status tag


## r4 (2013-02-08)

- [config.xml]: Updated for TEAM-Engine v4.
- [spsFunctions:getExceptionInfo]: Allow for multiple exceptions (with 0..* ExceptionText) 
  in exception reports.
- [sps:core-SPS.GetStatus-RequestWithSinceButServiceNoSupport.1]:
  Fixed XPath error: "Required item type of first argument of substring-after() 
  is xs:string; supplied value has item type xs:dateTime"


## r2 (2012-07-20)

- Update test suite for new xlink policy


## r1 (2012-04-05)


- Update index.html
- corrected version on config.xml


## r0 (2012-01-23)

- first revision
