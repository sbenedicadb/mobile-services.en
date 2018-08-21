---
description: To start using the Experience Cloud Device Co-op, contact your Adobe representative.
seo-description: To start using the Experience Cloud Device Co-op, contact your Adobe representative.
seo-title: Experience Cloud Device Co-op
title: Experience Cloud Device Co-op
uuid: 7413f5ca-d640-42b7-88da-cb2bf34c22a9
index: y
internal: n
snippet: y
translate: y
---

# Experience Cloud Device Co-op

To enable your mobile apps for the Experience Cloud Device Co-op, complete the following steps for the Experience Cloud iOS SDKs. 


>[!IMPORTANT]
>
>This functionality requires iOS SDK version 4.8.5 or later.



Starting in SDK version 4.16.1, Device Co-op members can opt their mobile device data out of the Experience Cloud Device Co-op. For more information see [ ADBMobile JSON Config](../configuration/json_config/json_config.md#concept_105FBD9EBABE4B21BD7D49687AB2D5BA) and the ` visitorAPI.js` method for [ isCoopSafe](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-coopsafe.html). 

>1. Implement the Adobe Mobile SDK.
>   For more information, see[ Core Implementation and Lifecycle](../getting_started/dev_qs.md#concept_13176B6E37F547D6935E37125F457972).>
>1. Enable your Experience Cloud ID.
>   For more information, see[ Experience Cloud ID](../marketing_cloud/mcvid.md#concept_581581B6726A422BAB8F44AE78E402AE).>
>1. Pass authenticated identities such as CRM IDs or hashed emails using one of the sync methods contained here.

>       [ Experience Cloud ID Service Methods](../marketing_cloud/mc_methods.md#concept_FFC0A9EA4C804CC5BAD5FB358F52A22A)