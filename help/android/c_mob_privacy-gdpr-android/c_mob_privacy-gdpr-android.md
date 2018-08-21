---
description: Experience Cloud Mobile SDKs provide General Data Protection Regulation (GDPR)-ready APIs for Controllers that allow users to retrieve locally stored identities and set opt status flags for data collection and transmission.
seo-description: Experience Cloud Mobile SDKs provide General Data Protection Regulation (GDPR)-ready APIs for Controllers that allow users to retrieve locally stored identities and set opt status flags for data collection and transmission.
seo-title: Privacy and General Data Protection Regulation
title: Privacy and General Data Protection Regulation
uuid: 0851830c-8dee-46bb-ad5c-59f699dd430b
index: y
internal: n
snippet: y
translate: y
---

# Privacy and General Data Protection Regulation


<a id="section_1A90E98BB29D425197097C6CA1220EC2"></a>


>[!IMPORTANT]
>
>GDPR is supported**only** in Mobile SDK version 4.16.0 or later. 



When Adobe provides software and services to an enterprise, Adobe acts as a data processor for any personal data it processes and stores as part of providing these services. As a data processor, Adobe processes personal data in accordance with your company’s permission and instructions (for example, as set out in your agreement with Adobe). 

As a data controller, you can use Adobe Mobile Services SDKs to support GDPR retrieve and delete requests from your mobile apps. 

For the Adobe Mobile SDK portions of your mobile apps, you can use the following settings and methods: 


* To retrieve data from the SDKs, and send this data to your servers, use the ` getAllIdentifiersAsync` method. 

  For more information, see [ Retrieving Stored Identifiers](../c_mob_privacy-gdpr-android/c_mob_gdpr_ret-stored-ids-android.md#concept_45DF30ADF75C497AA96A275C584A4118). 

* To set your opt status and help you with a GDPR data deletion request, use the following settings: 


    * ` privacyDefault`
    * ` setPrivacyStatus`


  For more information, see [ Setting the User's Opt Status](../c_mob_privacy-gdpr-android/privacy.md#concept_BF4AFEA7801F42E4B2A638A755BF11D5). 



## Additional Information {#section_7C7124C50D85469C8C8714533FB1A37D}


* For more information about GDPR, see [ GDPR and Your Business](https://www.adobe.com/privacy/general-data-protection-regulation.html).
* To see the GDPR API documentation, go to [ General Data Protection Regulation API](https://adobe.io/apis/cloudplatform/gdpr.html).
