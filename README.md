# Welcome
Welcome to my Github repo.

## Repos
All my repos are private. I'm happy to provide access to recruites or interviewers. Here is a short overview of what I have been working on.

### [schniesel-bestell](https://github.com/wulf0r/schniesel-bestell-rework)

Multichannel order managment for our family business [Schniesel-Kids](https://www.schniesel-kids.de). It unifies order handling for orders from Shopify, Etsy, E-Mail and Facebook.
Size: approx 35.000 loc

### Features

* order forms for manual entry
* order lists with search
* order status managment (New -> Paid -> Prepared -> Finished -> Sent)
* product label printing
* syncs products and orders from Shopify and Etsy
* automatically creates invoices in Sevdesk based on the orders in the app
* supports production planning
* automates customer notification
* prints DHL Labels from orders
* Transaction retrieval from Bank and Paypal for semi-automatically determining orders "paid" status


### History
The first iteration of this project went productive in 2015 and was built on Java with Apache Tapestry. The main goal then was to automatically determine paid status because most order were paid via bank transfer. Overtime the software grew to support the business and all the features listed above were gradually added. Notably, the existence of this software (and artikel-ui, see below) allowed us to very quickly migrate the shop from legacy EPages to Shopify.
In the year 2022, I ported everything over to Kotlin for backend and frontend. Notable in this project is that everything, such as data transfer objects, REST routes, frontend pages, that can be type safe, is type safe and everything that can be shared between frontend and backend is shared. 


#### Tech Stack
* Frontend: Kotlin/JS with Fomantic UI
* Backend: Kotlin Multiplatform with KTOR
* Persistence: H2 via JOOQ "SQL in Kotlin"
* Testing: Spock Framework and Selenium
* CI and deployment: Github actions build releases that are pulled into a docker image

#### Screenshots






