<h1>GrapthQL API Inventory</h1>
<h2>Brief:</h2>
<p> This is a NodeJs API that uses GraphQL to query a Postgresql database. This API and database willbe hosted on Heroku using their free tier for now, later we will migate the DB and put it on the tier </p>

<h3>API:</h3>
<p>This API will be fairly simple at the start. It will be used at the middle tier for a React Native mobile application, this app will be cross platform and in a future scope become a hybrid app running on both mobile and web platforms.

Heroku will be the host for the API, this will allow rapid growth, free hosting and be able to read from a fast speed.

This will be queried using GraphQl for fast simple data gathering, allow fast API dev with minimal entry points making developement simpler. </p>

<h2>Testing Framework: </h2>
<p> There is a large selection for testing frameworks that can be used but for testing the API we will be using:</p>

<h3> Unit Testing: </h3>

* Mocah 
* chakram

<h3> Performance Testing: </h3>

* artillery.io


<h3>Mocah:</h3>
Mocah is a javascript testing frameworking running on NodeJs and in browers, allowiung testing for Async functions easy.

[Mocah](https://mochajs.org/)

<h3>chakram:</h3>
Charkram is a REST API testing framework offerning BDD testing style and fully exploting promises.

[Chakram](http://dareid.github.io/chakram/)


<h2>Testing Best Practices </h2>


Different Test framworks:
Mocah, night watch, jasmine,karma phantomJS, Webdriver.io,Intern.io,qualitywatch.io

Mocha + Chakram = a good combo and simple (Charkam allow you to create custom functions and can be Data-Driven) {good API tests}

You should split out tests into page object design patterns

build the UI with automation in mind (name things with an actual name )

80 / 20 rule to test front end

mobile testing:
mocha + webdriver.io + appium = good combo 

perfomance testing:
phantommas + QualityMeter 


QualityWatcher gives good and fast testing breakdowns 

make sure there is a dashboard showing the quailty of the product etc



links:
https://www.youtube.com/watch?v=i4Eu3Cczkek

