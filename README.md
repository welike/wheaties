# wheaties

Eat your wheaties. A ruby gem for getting product information from merchant APIs (and scraping for additional data).

# Overview

A merchant-agnostic framework for the retrieval of product information, metadata, availability, pricing, and
community evaluation (ratings/reviews) by way of official APIs and web scraping. When content is not available
through official APIs it will be augmented with scraped data and potentially data from other merchants.

# Values

There are some values that we wish to embrace during the development of wheaties.

1. **Simplification &amp; ease of use.**

  The interface should be simple and it should be easy to use. The documentation should be simple and clear. At no
  point should this framework get in the way of the projects of the people who are using it.
  
2. **Reliability.**

  Companies will be using this to build products so it should be reliable. Errors and outages cost companies money,
  and many of the companies using this will be small businesses (often run by only a few people) and saving them money
  so they can rapidly build products is the primary goal.

3. **Compatibility.**

  One of the biggest motivators to make wheaties was that merchants are not compatible with each other. They offer
  different APIs, different data, and exist to compete with each other. It is our goal to make them compatible by
  unifying access to them for our own projects.
  
4. **Kindness, recognition and collaboration.**

  Developers should be treated with respect. They should be kind to each other, even when conflict arises. Additionally,
  efforts made should be recognized and rewarded. Collaboration is the heart of the experience, allowing a quality
  framework to rise and grow over time.

# Helping Out

Yes, we want your help.

But how can you help?

1. **Donate.**

  This is the easiest way to help. You can contribute to the development fund, which will help us continue development
on this framework instead of taking on paid contracts. It will let us hire other people to help too.

2. **Submit bug fixes and small enhancements.**

  This is the second easiest way to help. See an Issue that needs fixing? Jump in, fork the repository, fix the bug, and
submit a Pull Request. It will benefit everyone. Also, any kind of small enhancement or improvement is also a great way
to help out. Perhaps there needs to be an additional option, or some parsed data is missing that is useful. Fork the
repository, add it in, and submit a Pull Request.

3. **Submit more significant features.**

  As they say... it takes a village.

  Want to see quality testing? Jump in and add/improve the rspec specs.
  Want to see a new merchant? Jump in and mimmic the foundations of the other merchant interfaces.
  Want to make the code more reusable? Find commonalities, extract and refactor.

4. **Tell others.**

  This is a free framework (with exception to donations perhaps), and so ultimately we're not in the game of self-promotion.
But if you'd like to see this framework proliferate, telling others about it will certainly help with that. Let your 
favorite mailing list know about the project, and it will give it a boost in terms of community interest (and hopefully
contributions to bug fixing and feature support).

# FAQ

1. **Why the name wheaties?**

  I thought it best exemplified products and marketing, and as an aging product it indicates an 
opportunity to search inventory, price compare, and otherwise is a fun but unique name for the gem and
the repository.

2. **What merchants are supported?**

  Initially, wheaties will support Amazon Product Search API (and scraping for pricing data since the API
  does not provide it comprehensively), Newegg, and Walmart. Once the framework is supporting these completely,
  we will consider additional merchants on a case-by-case method based on demand.

3. **Some of these merchants already have an API, why do we need wheaties?**

  Merchants that do offer an API do not standardize their interfaces with each other. It forces you, the developer,
  to write code to individually support them. Even if you find a library that exists for each one, each of those
  libraries are also inconsistent with each other. Some merchants don't even have an API, forcing you to scrape the
  contents from their websites.
  
  The reality is that most of the data between merchants is the same. The data is about product info, their availability,
  their pricing, and potentially their community's perspective of those products (reviews, ratings, etc). The differences
  are mostly in the way that the API operates (authentication strategies and styles), the nomenclature, and the amount
  of information provided.
  
  The *wheaties* framework should serve to help unify some of these differences into a common and **simplified**
  format and interface, and will make it easier to integrate into your own applications.

4. **Isn't web scraping bad?**
 
  While we think that abusive scraping to order to fraud or cheat a service or merchant
  from their data in a competitive manner is bad, we do think that scraping to get access to data that could ultimately
  benefit that service or merchant is not bad.
  
  In otherwords, if you web scrape to steal data from a site that exists
  only because it has that data and you are building a product to directly compete with them, then this is wrong. Scraping
  data from a website that lists places to change a baby's diaper just to make a competing site that lists places to change
  a baby's diaper is wrong.
  
  But if you are building something that helps that business in some way, such as a merchant who sells products and using
  their data on your site allows people to somehow buy more things from that merchant, then this is a good use of scraping.
  
  Abusive scraping, such as the kind that hits a service with excessive traffic and degrading their service quality, is
  never acceptable.
  
