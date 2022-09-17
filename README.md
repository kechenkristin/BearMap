# BearMap
## About The Project
This project is from UCB CS61B fall 2018 project4.
https://sp18.datastructur.es/materials/proj/proj3/proj3
It is a web mapping application inspired by a former TA’s time on the Google Maps team and the OpenStreetMap project, from which the tile images and map feature data was downloaded.
Working with the back end - the web server that powers the API that the front end makes requests to. 

## Features
1. Scrolling and Zooming
![avatar](https://github.com/kechenkristin/imagesGitHub/blob/main/projects/BearMap/zoom1.png)
![avatar](https://github.com/kechenkristin/imagesGitHub/blob/main/projects/BearMap/zoom2.png)
![avatar](https://github.com/kechenkristin/imagesGitHub/blob/main/projects/BearMap/zoom4.png)
![avatar](https://github.com/kechenkristin/imagesGitHub/blob/main/projects/BearMap/zoom3.png)


2. Route finding (similar to Google Maps) and Navigation

Double click a start point and end point to find the shortest path.
![avatar](https://github.com/kechenkristin/imagesGitHub/blob/main/projects/BearMap/shorestPath1.png)
![avatar](https://github.com/kechenkristin/imagesGitHub/blob/main/projects/BearMap/shorestPath3.png)
![avatar](https://github.com/kechenkristin/imagesGitHub/blob/main/projects/BearMap/shorestPath2.png)


3. Autocomplete

![avatar](https://github.com/kechenkristin/imagesGitHub/blob/main/projects/BearMap/auto.png)


## Build With
SAX parser
OSM XML
JAVA Collection framework

## Implementation Ideas
1. Scrolling and zooming: The user’s web browser provides a URL to the Java program, and the Java program will take this URL and generate the appropriate output by using rastering algorithm, and the output will displayed in the browser. 

2. Working with a real world dataset presented in the OSM XML file format, using SAX parser( an “event-driven online algorithm for parsing XML documents” ) to parse XML element into java object, and create a graph datastructure to represent the info for the project.

3. Implementing A* algorithm to find the shortest path and using the A* search route to generate a sequence of navigation instructions. 

4. An Autocomplete system where a user types in a partial query string, like “Mont”, and is returned a list of locations that have “Mont” as a prefix. Implementing this feature by using trie data structure, traversing to the node that matches the prefix (if it exists) and then collect all valid words that are a descendant of that node. 



## Usage
Build the project, run MapServer.java and navigate your browser (Chrome preferred; errors in other browsers will not be supported) to localhost:4567
If you get a “404 Not found” error, you can open src/static/page/map.html manually by right clicking and going to Open In Browser in IntelliJ.


## Contact

Author: Kechen Liu

Email: kechenkristin@gmail.com

Project Link: https://github.com/kechenkristin/BearMap










