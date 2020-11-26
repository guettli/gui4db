# List of ways to get a web GUI for a database

This is an opinionated list. 

I would like to develop a new web application.

Here I am listing tools to develop a web applications. This helps me to structure my research.

# My Background

I develop Django applications since 2008, this means 12 years.

Django is great, and it is mature. I love the language Python.

But time has changed. Maybe it is time to switch?

# Database

At the heart of every web application is a database.

I worked with CSV files, sqlite, ZODB (an object oriented database for Python), MongoDB, MySQL and PostgreSQL.

My favorite database is PostgreSQL.


# Frontend

Sending HTML over the wire is still very common. There are many productive applications created with
Django, PHP, Rails, ...

This way is perfectly fine. There are tools to help you to write modern application this way. A list
of JS libraries which help here are on my [HTML over the wire](https://github.com/guettli/html-over-the-wire) page.

But new applications get usualy build with Angular, React or Vue these days.

At the moment I would choose Vue. But this is not settled yet.

If I go the JSON-over-the-wire approach, I need a way to get an http API for my data inside PostgreSQL.

# What kind of http API?

Again, I am open minded and not settled yet.

Here are some required features:

* The API should have a parsable description, so that introspection is possible.

OK, up to now I only have this requirement.

This means it could be:

* [GraphQL](https://en.wikipedia.org/wiki/GraphQL)
* [OpenAPI/Swagger](https://en.wikipedia.org/wiki/OpenAPI_Specification)
* [gRPC](https://en.wikipedia.org/wiki/GRPC)
* [Thrift](https://en.wikipedia.org/wiki/Apache_Thrift)
* ...

# PostgREST

Provides OpenAPI via a thin wrapper written in Haskel.

[PostgREST](http://postgrest.org/)

# Django Rest Framework

DRF provides OpenAPI (See [Schemas](https://www.django-rest-framework.org/api-guide/schemas/))

[django-restql](https://github.com/yezyilomo/django-restql) provides GraphQL




# Prisma 2

[Prisma2](https://www.prisma.io/) 

But somehow I am unsure if this is cool. Very young (started 2019, after Prisma1 and Graphcool).

Works for several databases, not just PG. 

Provides ORM, not OpenAPI or GraphQL.



# Hasura

[Hasura at github](https://github.com/hasura/graphql-engine/)

Since 2018

Looks good.

Implemented in Haskel+JS.

# PostGraphile 

[PostGraphile Instant GraphQL API](https://www.graphile.org/postgraphile/)

Since 2016

Implemented in JS+Typescript.

