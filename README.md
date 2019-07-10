# Automate Wishlist with Selenium & Cucumber (BDD)

## Dependencies

- [Cucumber](https://github.com/cucumber/cucumber)
- [Junit](https://mvnrepository.com/artifact/junit/junit/4.12)
- [Selenium](https://github.com/SeleniumHQ/selenium)
- [Webdrivermanager](https://github.com/bonigarcia/webdrivermanager)

## Set up

- clone repository
  ```
  git clone https://github.com/Nidhisachan/selemiumAutomation.git
  cd /selemiumAutomation
  mvn clean install
  ```
- Test result generation on following path: /target/cucumber/index.html

![image](https://lh3.google.com/u/0/d/1cdSlVZIn_A2d6n8mkvRI4xdcNV7HyxSF=w3048-h1548-iv1)

## Folder Structure

```
├── README.md
├── pom.xml
├── src
│   └── test
│       ├── java
│       │   └── seleniumassignment
│       │       └── automation
│       │           ├── config
│       │           │   ├── RunCucumberTest.java
│       │           │   └── SharedContext.java
│       │           ├── pom
│       │           │   ├── actions
│       │           │   │   └── AbstractPage.java
│       │           │   ├── pages
│       │           │   │   ├── HomePage.java
│       │           │   │   ├── MyWishListPage.java
│       │           │   │   ├── ProductDetails.java
│       │           │   │   └── SearchResults.java
│       │           │   └── uielements
│       │           │       ├── HomePageElements.java
│       │           │       ├── ProductDetailPageElements.java
│       │           │       ├── SearchResultPageElements.java
│       │           │       └── WishListPageElements.java
│       │           └── stepdefs
│       │               ├── CommonSteps.java
│       │               ├── MyWishListSteps.java
│       │               └── SearchProductSteps.java
│       └── resources
│           └── seleniumassignment
│               └── automation
│                   ├── MyWishList.feature
│                   └── SearchProduct.feature
└── target
```

## Folder Description

- **_config:_** Defining cucumber class runner and cucumber options.
- **_pom:_** Defining page locators, page actions.
- **_stepdefs:_** Defining step definitions of the respective feature files.
- **_resources:_** Defining feature files in gherkin.
- **_target:_** Test report generation happens in this folder.

