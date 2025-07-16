# Selenium Notes


## Setting Driver
```java
System.setProperty("webdriver.gecko.driver", "/usr/bin/geckodriver");
		driver = new FirefoxDriver();
```
/usr/bin/geckodriver <- Path to geckodriver



- Starting in Headless Mode without gui
```java
FirefoxOptions fOptions=new FirefoxOptions();
fOptions.addArguments("--headless");
WebDriver driver= new FirefoxDriver(fOptions);
```

## Navigation

- To Open Up Browser With a Specific Url:

```java
driver.get(baseUrl);

```
- To Navigate to a url:
```java
driver.navigate().to(url);
```
There is also:
```java
driver.navigate().back();
//Forward
driver.navigate().forward();
//Refresh
driver.navigate().refresh();
```

## Finding Element

```java
 driver.findElement(By)
 driver.findElements(By)
```
- Using Id By.id("id")

- Using Xpath By.xpath("xpath")
    - Xpath references: [Xpath Url](https://www.w3schools.com/xml/xpath_syntax.asp)

- Using tag name By.tagName()


## Documentation

[Selenium Docs](https://selenium.dev)

