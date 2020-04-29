# Access Galway
## CS7IS1- Access Galway- Knowledge and Data Engineering
**Team H**

## Introduction
For this project we have built an interactive ontology-driven application, based on three different datasets (which do not have a RDF version already available). The datasets are from Ireland’s [Open Data Portal](https://data.gov.ie/). A set of ten template questions have been defined that the users of our application could use to get specific answers from the datasets.

The application is based on an ontology we developed from the three datasets (Playground locations, blue badge parking locations and sports facilities in Galway) called “Access Galway” which represents three major aspects - playgrounds, sports facilities and blue badge parking in the city. The queries that can be posed to the ontology revolve around providing accessibility features and parking to less-abled citizens when they or the people they are accompanying visit playgrounds or other sports facilities in Galway.

## Approach to Ontology Modelling

### Description of Competency Questions that ontology answers

Our queries use coordinates of a location, and gives user the option to choose the range of distance between which they want to find places of their interest. Their interest here is again given as an option to user while querying, which could include options such as playground parking within estate near soccer pitches (as mentioned in query 5), certain surface type of playground near by blue badge parkings (as mentioned in query 2) or even a more specific complex query like a sports facility with a specific equipment near a blue badge parking (as mentioned in query 6).
Our querying interface not only allows user to input the specific instance of their interest, but also allows user to decide the range of distance by which they want to access a facility in Galway.

### Description of Datasets selected for application

Description of Datasets selected for application: 
For the project, we had selected three different datasets from [here](data.gov.ie) namely,

1. Galway City Blue Badge Parking Locations (71 entries)
2. Galway City Playground Locations (30 entries)
3. Galway City public Sports Facilities (47 entries)

These datasets are published by Galway City Council, and the common theme of the datasets is the city ‘Galway’. All these three datasets have common data and object properties, namely Cartesian coordinates (X and Y), Irish Transverse Mercator (ITM), Irish Grid (IG), Geographic Coordinate system (Latitudes and Longitudes) and Object IDs.
The datasets 1 and 2 were updated as recently as 2015-10-20. The dataset 3 was updated on 2019-08-21.

Future applications for a more effective tool to use in Galway could use other datasets provided by Galway City Council, like Piers and Harbours of Galway County, Galway County Fire stations, Galway County Council Administrative Buildings. 

### Running the Application

    1. Open the directory containing the code
    2. Open terminal or an IDE (Visual Studio code)
    3. Run the command ```npm install``` (This installs the required packages)
    4. Run the command ```ng serve``` (This will open the app in http://localhost:4200/)

### Requirements

   1. Angular CLI should be installed. To know more refer link https://angular.io/guide/setup-local
   2. Sparql end point should be set up. (Here apache fuseki-server is used as sparql endpoint- http://localhost:3030/dataset/sparql). Create a data set with the ttl files in fuseki server and change the endpoint in the code
