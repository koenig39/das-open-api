# DAS

Open APi version: 3.0

Files are  located in the “Public” GitHub repository without security API key.

To make a real request, you will have to create API key in Azure Cloud Function  


| Link | Description |
| :--- | :--- |
| [https://raw.githubusercontent.com/koenig39/das-open-api/v1/openapi.yml](https://raw.githubusercontent.com/koenig39/das-open-api/v1/openapi.yml) | Production API |
| [https://raw.githubusercontent.com/koenig39/das-open-api/dev/openapi.yml](https://raw.githubusercontent.com/koenig39/das-open-api/dev/openapi.yml) | Development version with all latest features |

How to use: 

\(In browser\) Open [https://editor.swagger.io/](https://editor.swagger.io/) and import the required API version file.

You can also open API file in “Postman”.  


## Description

Formations: represent as numbers eg: \(“UB”:0, “MB”: 1, “”...\)  
  
  


DAS function input parameters: 

* Polygon
  * coordinated
* Interpolation
* Resolution
* Formations

## Tests and Validation

**Input Validation**

Polygon

* Coordinates needs to be correct type \(-+90,-+180\)
* \([https://stackoverflow.com/questions/3518504/regular-expression-for-matching-latitude-longitude-coordinates](https://stackoverflow.com/questions/3518504/regular-expression-for-matching-latitude-longitude-coordinates)\)
* Minimum size of the polygon \(area\)
* Maximum size of the polygon \(area\)
* Polygon coordinates forms valid polygon \(shapely Polygons have is\_valid\)

    Interpolation 

    Resolution

* min/max values

    Formations

* If formation exists 
* Formation set contains only adjacent formations
* Default formation

        - min/max count 

        - default returned formation if input is empty

        - is correct formation type 

            - is allowed type of the formation

        - dominant formation is set and included in input

        - returned name is correct

        - dominant layer satisfies data requirements

