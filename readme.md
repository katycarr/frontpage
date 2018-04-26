# FrontPage #

FrontPage uses several APIs and text analyzers to allow users to create a customized newsfeed. The Rails backend pulls from [News API](https://newsapi.org/), scrapes each url using Nokogiri, then posts the text of the article to the [Aylien Text Analysis](https://aylien.com/text-api/) API to find out what it's about. It also uses the readingtime gem to estimate how long it will take to read the article.

The front end is built with React and Redux to manage state.

## Domain
![schema](/schema.png)

## User Stories
* As a user, I can sign up, log in, and log out
* As a user, I can select, edit, and delete my tracked topics
* As a user, I can login and see new articles related to my topics
* As a user, I can save stories to read later

## Frameworks & Libraries

* APIs
  * [News API](https://newsapi.org/)
  * [Aylien Text Analysis](https://aylien.com/text-api/)
  * [Watson NLU](https://www.ibm.com/watson/services/natural-language-understanding/)
  * [DBpedia lookup](https://github.com/dbpedia/lookup)
* Gems
  * jwt
  * Odyssey
  * readingtime
  * nokogiri
  * ruby-readability
  * aylien_text_api
  * watson-api-client
  * active_model_serializers
  * activerecord-import
