<h1>GrapthQL API Inventory</h1>

## Table Of Contents:
- [Brief](#Brief)
- [API](#API)
- [Testing Framework](#Testing-Framework)
  - [Unit Testing](#Unit-Testing)
  - [Performace Testing](#Performance-Testing)
  - [Testing Best Practices](#Testing-Best-Practices)
- [Little Notes](#Little-Notes)
- [Useful Links](#Useful-Links)


<h2>Brief:</h2>
<p> This is a NodeJs API that uses GraphQL to query a Postgresql database. This API and database willbe hosted on Heroku using their free tier for now, later we will migate the DB and put it on the tier </p>


<h3>API:</h3>
<p>This API will be fairly simple at the start. It will be used at the middle tier for a React Native mobile application, this app will be cross platform and in a future scope become a hybrid app running on both mobile and web platforms.

[Heroku](https://www.heroku.com) will be the host for the API, this will allow rapid growth, free hosting and be able to read from a fast speed.

This will be queried using GraphQl for fast simple data gathering, allow fast API dev with minimal entry points making developement simpler. </p>

<h2>Testing Framework:</h2>
<p> There is a large selection for testing frameworks that can be used but for testing the API we will be using:</p>

<h3>Unit Testing:</h3>

* [Mocah](https://mochajs.org/)
* [Chai](https://www.chaijs.com/)

<h3>Performance Testing:</h3>

* [Artillery](https://artillery.io/)


<h3>Mocah:</h3>
<p>
Mocah is a javascript testing frameworking running on NodeJs and in browers, allowiung testing for Async functions easy.</p>


<h3>Chai:</h3>
<p>Chai is a BDD / TDD assertion library for node and the browser that can be delightfully paired with any javascript testing framework.</p>


<h3>Artillery:</h3>
<p>Artillery is a modern, powerful & easy-to-use load testing and functional testing toolkit. Use it to ship scalable backends, APIs & services that stay performant & resilient under high load.</p>


<h2>Testing Best Practices:</h2>

<h3>Page Object Model (POM):</h3>
<h4>Whats a POM:</h4>

<p>POM is a design pattern to create Object Repository for UI elements under this model, for each web page in the application, there should be corresponding page class. 

This Page class will find the WebElements of that web page and also contains Page methods which perform operations on those WebElements.

Name of these methods should be given as per the task they are performing, i.e., if a loader is waiting for the payment gateway to appear, POM method name can be waitForPaymentScreenDisplay().

<h4>Advantages of POM</h4>

1. Page Object Pattern says operations and flows in the UI should be separated from verification. This concept makes our code cleaner and easy to understand.

2. The Second benefit is the object repository is independent of test cases, so we can use the same object repository for a different purpose with different tools. For example, we can integrate POM with TestNG/JUnit for functional Testing and at the same time with JBehave/Cucumber for acceptance testing.

3. Code becomes less and optimized because of the reusable page methods in the POM classes.

4. Methods get more realistic names which can be easily mapped with the operation happening in UI. i.e. if after clicking on the button we land on the home page, the method name will be like 'gotoHomePage()'.
</p>




<h2>Little Notes:</h2>

* Mocha + Chai = a good combo and simple 
* Charkam was gonna used but active support has was stopped in 2018

* You should split out tests into page object design patterns

* build the UI with automation in mind (name things with an actual name )

* 80 / 20 rule to test front end

* mobile testing:
mocha + webdriver.io + appium = good combo 

* make sure there is a dashboard showing the quailty of the product etc


<h2>Useful Links:</h2>

[Page Object Model (POM) & Page Factory: Selenium WebDriver Tutorial](https://www.guru99.com/page-object-model-pom-page-factory-in-selenium-ultimate-guide.html)


[Full Stack Testing with Node.js by Stacy Kirk, Quality Works](https://www.youtube.com/watch?v=i4Eu3Cczkek)

[JavaScript — Unit Testing using Mocha and Chai](https://codeburst.io/javascript-unit-testing-using-mocha-and-chai-1d97d9f18e71)

[Node.js & JavaScript Testing Best Practices (2019)](https://medium.com/@me_37286/yoni-goldberg-javascript-nodejs-testing-best-practices-2b98924c9347)

