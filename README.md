# Olapictechtest
This is where my technical test files and answers to questions can be seen. Below can be found the answers to the questions and validation test issue and solution.

Website creation:
Once I read up on the API documentation, I started to research best grid layouts which is when I came across the “grid” layout type, but upon retrieving the images I found that there were over 10 images and all the of them had to be displayed.

At this point I started to investigate arrays which is where I found the Owl Carousal, this allows to change images on a loop, once set up correctly and uses an array to do so. Alongside that I used jQuery and AJAX to make the GET requests. Which then allowed me to receive back the JSON format form the API.


Q1 -- Integration Inquiry
"Is there an Olapic integration with Salesforce Commerce Cloud? We are in the process of moving to SCC; if we decided to integrate Olapic, how "would we go about doing that?”

A1: Yes, there is an integration between Olapic and Salesforce, to start the integration process please follow the link: https://www.salesforce.com/products/commerce-cloud/partner-marketplace/partners/olapic/ , and on the left hand side click on the “DOWNLOAD INTEGRATION” button which will start to link your SCC and Olapic product.

Rationale/Sources: Having search for SCC and Olapic, links below came up and can be used to help the customer.
https://www.olapic.com/partners/salesforce-commerce-cloud/ 
https://www.salesforce.com/products/commerce-cloud/partner-marketplace/partners/olapic/ 

Q2 -- Site Performance Issue
"We are noticing that our page is loading slowly. We have 50 high-resolution images loading in the Olapic carousel and we'd like to speed it up!”

A2: We can certainly help with that, please go to our API documentation where you can find information on the carousal and you can further apply customisations to the code itself. The links are as follows: http://developer.olapic.com/articles/tutorial-apiv2-carousel-example.html (example of the carousel) , http://apiv2-docs.photorank.me/index.html#top (API documentation)  and https://github.com/Olapic/PublicDocs (public documents). In order to reduce latency please see http://developer.olapic.com/articles/widget-load-optimization-guide.html , which gives guidelines and provides instructions on how to improve speed while also utilising our SDK.

Rationale/Sources: I found the links below by just searching and looking though the API documentation, these would help in resolving the issue above.
http://developer.olapic.com/articles/tutorial-apiv2-carousel-example.html
http://apiv2-docs.photorank.me/index.html#top
https://github.com/Olapic/PublicDocs
http://developer.olapic.com/articles/widget-load-optimization-guide.html 

Q3 -- Customization Request
“Unless Olapic JS widgets support IE8, it looks like we may have to take our business elsewhere. What can you do to make this happen?”
Note: Olapic widgets only support IE9+ and modern browsers. Olapic API is often used as an alternative to Olapic JS widgets.

A3: Thank you for reaching out and you as a customer are valuable for us and having recognised that some customers might be running on IE9 or less, we have made our API compatible with browsers below IE9. By using the API you still get the functionality in some cases customers have used it for widgets. Please have a look at our API docudmentation to get started, if you need anything else please feel free to contact us again.
http://apiv2-docs.photorank.me/index.html#top

Rationale/Sources: Guiding them to the API will show that we still care about their business and will provide support where possible

Q4 -- Unhappy Customer
"Our widgets are down! You sent us an email saying our new API key is ready and now we're getting a message saying API key expired!”
Note: Due to a bug on our side, the API key that was generated for them was expired at the time they received it. The new API key is now ready for them to access in their Olapic account.

A4: I sincerely apologise for the inconvenience this has caused, please find your new key: XXX, please go ahead and try this key and if this still doesn’t work then please do get in contact again and I will be more than happy to help you. Your old key didn’t work due to a bug on our side which we are now working on to resolve.

Rationale/Sources: This is something that we have done incorrectly and we need to be transparent with the customer and accept that its our fault but also go the next step and ask them to contact us if anything else goes bad, as good customer service is key.

Validation results/problem:
1. Parsing error created by " Shorts Red" on line 139
2.	Cvc-pattern-valid: Value 'APTS-02 Blue' Is Not Facet-valid With Respect To Pattern '[\S]+' For Type 'UniqueIdType'., Line '54', Column '48'.
3.	Cvc-type.3.1.3: The Value 'APTS-02 Blue' Of Element 'ProductUniqueID' Is Not Valid., Line '54', Column '48'.

Validation solution: 
1. Remove "Shorts Red" as that didnt allow parsing, after which is worked fine.
2 & 3. Remove the word “Blue” as in the schema it only asks for size and this should fix the issue.

