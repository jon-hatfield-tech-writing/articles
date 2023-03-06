![data icons](../images/data-in-2023-icon.png)

# Data in 2023
## A summary for IT professionals
### by Jon Hatfield - Mar 1, 2023

Data is the ultimate source of truth for any system and it's increasingly pooled on the internet, 
becoming larger and more complex. It is important for developers, business analysts and even general 
users of the internet to understand how this data is stored and used.

## Storage

The storage options of SQL and noSQL remain the most relevant. Whilst SQL is the older technology it is 
still the best option for structured data and transactions, providing the amount of data is relatively 
small e.g. under 100 million rows per table. For fast performance, simpler data structures and higher 
volumes, noSQL is the best option. Cloud implementations such as
[AWS RDS](https://aws.amazon.com/rds)
and
[DynamoDB](https://aws.amazon.com/dynamodb/)
continue to
replace on-premises databases unless there is a good reason not to, such as extremely high security requirements 
or usage of deprecated technology. Integration technology such as
[AWS Direct Connect](https://aws.amazon.com/directconnect/)
can be used to combine the two approaches.

## Maintenance

Cloud services such as
[AWS](https://aws.amazon.com/)
and CI/CD tools such as
[Jenkins](https://www.jenkins.io/)
alleviate the need for error-prone manual adjustments of
data structure and content; scripts can be run automatically and and managed with version control. Cloud hosted 
databases such as
[RDS](https://aws.amazon.com/rds/)
also abstract away much of the responsibility of database tuning and other low level 
system admin tasks. At the code level, data migration tools such as
[Flyway](https://flywaydb.org/)
help to keep code automatically in sync with the data. These advancements are making data maintenance 
more automated and streamlined.

## Monitoring

Most enterprise systems have a monitoring setup such as an
[ELK stack](https://www.elastic.co/what-is/elk-stack)
or
[Datadog](https://www.datadoghq.com/)
to present application data, metrics and logs. The data consolidation and visualisation features of dashboards are
increasingly important given the growth in the typical number of data sources; data is now likely to come from modern
microservices architectures as opposed to single monoliths. It is also expected that machine learning
and artificial intelligence will become more common additions to dashboards, allowing yet more insight and analysis.

## Software Development

Applications can connect to cloud data with SDKs e.g.
[AWS SDK for Python](https://aws.amazon.com/sdk-for-python/).
Data management through code is simplified with frameworks such as
[Java Spring Batch](https://spring.io/batch)
and
[Hibernate](https://hibernate.org/).
Instrumentation libraries such as
[Micrometer](https://micrometer.io/)
and
[Actuator](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#actuator)
are also useful for exposing and pushing metrics to external dashboards. Custom database queries within
application code are still common, especially for backing RESTful APIs.

## Data Transfer

With decoupled microservices becoming the standard choice of architecture, along with RESTful APIs and decoupled
front ends, there is an increased need for integration. Messaging systems such as
[Kafka](https://kafka.apache.org/)
are an effective way to asynchronously decouple backend microservices and handle large volumes of data. It is also common for companies 
to represent their data as a suite of RESTful APIs and as such there are various documentation standards emerging to
facilitate this as yet unstandardised area:
[Google API design](https://cloud.google.com/apis/design),
[JSON API](https://jsonapi.org/)
and
[Swagger](https://swagger.io/solutions/api-documentation/)
are examples. In terms of the front end,
[React](https://reactjs.org/)
is a popular way to receive data; it can elegantly update the DOM via RESTful API calls or, for bidirectional communication, via
[WebSockets](https://socket.io/).

It's an exciting time of data growth in all industries, from online banks such as
[Monzo](https://monzo.com/)
to multiplayer video games such as
[Call Of Duty Warzone](https://www.callofduty.com/uk/en/warzone).
Familiar technologies lie at the foundation however there is an 
increasing array of tools and techniques to integrate and manipulate the data.