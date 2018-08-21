---
description: The products variable cannot be set by using processing rules. In the iOS 4.x SDK, you must use a special syntax in the context data parameter to set products directly on the server call.
seo-description: The products variable cannot be set by using processing rules. In the iOS 4.x SDK, you must use a special syntax in the context data parameter to set products directly on the server call.
seo-title: Products Variable
solution: Marketing Cloud,Analytics
title: Products Variable
topic: Developer and implementation
uuid: afcc6253-0e23-4549-80d0-3d3305c93a98
index: y
internal: n
snippet: y
translate: y
---

# Products Variable

To set the *` products`* variable, set a context data key to ` "&amp;&amp;products"`, and set the value by using the syntax that is defined for the [ products ](http://microsite.omniture.com/t2/help/en_US/sc/implement/?f=c_products) variable: 

```
[contextData setObject:@"Category;Product;Quantity;Price[,Category;Product;Quantity;Price]" forKey:@"&amp;&amp;products"];
```
For example: 

```
//create a context data dictionary 
NSMutableDictionary *contextData = [NSMutableDictionary dictionary]; 
 
// add products, a purchase id, a purchase context data key, and any other data you want to collect. 
// Note the special syntax for products 
[contextData setObject:@";Running Shoes;1;69.95,;Running Socks;10;29.99" forKey:@"&&products"]; 
[contextData setObject:@"1234567890" forKey:@"m.purchaseid"]; 
[contextData setObject:@"1" forKey:@"m.purchase"]; 
 
// send the tracking call - use either a trackAction or TrackState call. 
// trackAction example: 
[ADBMobile trackAction:@"purchase" data:contextData]; 
// trackState example: 
[ADBMobile trackState:@"Order Confirmation" data:contextData]; 

```
*` products`* is set directly on the image request, and the other variables are set as context data: 
![](assets/products-bloodhound.png) All context data variables must be mapped by using processing rules: 
![](assets/map-products.png) You do not need to map the *` products`* variable using processing rules because it is set directly on the image request by the SDK. 