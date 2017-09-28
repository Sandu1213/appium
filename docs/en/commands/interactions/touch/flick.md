# Tap

Flick on the touch screen using finger motion events
## Example Usage

```java
// Java
TouchActions action = new TouchActions(driver);
action.flick(element, 1, 10, 10);
action.perform();

```

```python
# Python
actions = TouchActions(driver)
actions.flick_element(element, 1, 10, 10)
actions.perform()

```

```javascript
// Javascript
// webdriver.io example
driver.touchFlick('<ELEMENT_ID>', 1, 10, 10);



// wd example
await element.flick(1, 10, 10);

```

```ruby
# Ruby
@driver.touch_action.flick(element, 1, 10, 10).perform

```

```php
# PHP
// TODO PHP sample

```

```csharp
// C#
// TODO C# sample

```



## Client Docs

 * [Java](https://seleniumhq.github.io/selenium/docs/api/java/org/openqa/selenium/interactions/touch/TouchActions.html#flick-org.openqa.selenium.WebElement-int-int-int-) 
 * [Python](https://seleniumhq.github.io/selenium/docs/api/py/webdriver/selenium.webdriver.common.touch_actions.html#selenium.webdriver.common.touch_actions.TouchActions.flick_element) 
 * [Javascript (WebdriverIO)](http://webdriver.io/api/protocol/touchFlick.html) 
 * [Javascript (WD)](https://github.com/admc/wd/blob/master/lib/commands.js#L1513) 
 * [Ruby](http://www.rubydoc.info/gems/selenium-webdriver/Selenium%2FWebDriver%2FTouchActionBuilder:flick) 
 * [PHP](https://github.com/appium/php-client/) 
 * [C#](https://github.com/appium/appium-dotnet-driver/) 

## Support

### Appium Server

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
| iOS | [XCUITest](/docs/en/drivers/ios-xcuitest.md) | 9.3+ | 1.6.0+ | All |
|  | [UIAutomation](/docs/en/drivers/ios-uiautomation.md) | 8.0 to 9.3 | All | All |
| Android | [UiAutomator2](/docs/en/drivers/android-uiautomator2.md) | ?+ | 1.6.0+ | All |
|  | [UiAutomator](/docs/en/drivers/android-uiautomator.md) | 4.2+ | All | All |
| Mac | [Mac](/docs/en/drivers/mac.md) | ?+ | 1.6.4+ | All |
| Windows | [Windows](/docs/en/drivers/windows.md) | 10+ | 1.6.0+ | All |

### Appium Clients 

|Language|Support|
|--------|-------|
|[Java](https://github.com/appium/java-client/releases/latest)| All |
|[Python](https://github.com/appium/python-client/releases/latest)| All |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| All |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| All |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| All |
|[PHP](https://github.com/appium/php-client/releases/latest)| All |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| All |

## HTTP API Specifications

### Endpoint

`POST /session/:session_id/touch/flick`

### URL Parameters

|name|description|
|----|-----------|
|session_id|ID of the session to route the command to|

### JSON Parameters

|name|type|description|
|----|----|-----------|
| element | string | ID of the element where the flick starts |
| xoffset | number | The x offset in pixels to flick by |
| yoffset | number | The y offset in pixels to flick by |
| speed | number | The speed in pixels per seconds |

### Response

null

## See Also

* [JSONWP Specification](https://github.com/SeleniumHQ/selenium/wiki/JsonWireProtocol#sessionsessionidtouchflick)