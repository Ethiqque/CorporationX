# CorporationX

![URL](https://pbs.twimg.com/media/FuE_T4EWwAIgxzw.jpg:large)

CorporationX (CorpX) is a social network tailored for management and fundraising startups, offering centralized communication and collaboration tools. The platform provides real-time notifications, data-driven analytics, and efficient link management, enabling seamless business operations. With features like an infinite-availability news feed, activity achievements, and a dual message payment system, CorpX drives productivity for its users.

CorpX enhances startup fundraising by facilitating seamless team coordination and data-driven decision-making. Its real-time alerts keep users informed of key updates across multiple platforms, while its powerful dashboard offers a comprehensive view of performance metrics. By integrating flexible payment options and an intuitive URL shortener, CorpX streamlines communication and resource management.

## Microservices

* [**User Service**](https://github.com/CorporationX/user_service/tree/basilisk-master-bc4) - A comprehensive service managing user information, authentication, and authorization.
* [**URL-Shortener Service**](https://github.com/CorporationX/url_shortener_service/tree/basilisk-master-bc4-ethiqque) - Service to convert long URLS with 30+ symbols to short URL with 4+ symbols
* [**Project Service**](https://github.com/CorporationX/project_service/tree/basilisk-master-bc4) - Handles the creation, management, and collaboration of various projects.
* [**Post Service**](https://github.com/CorporationX/post_service/tree/basilisk-master-bc4) - Facilitates the creation and management of user-generated posts and content.
* [**Payment Service**](https://github.com/CorporationX/payment_service/tree/basilisk-master-bc4) - A web system for handling and monitoring financial transactions and book checkouts.
* [**Analytics Service**](https://github.com/CorporationX/analytics_service/tree/basilisk-master-bc4) - Provides analytical insights and data reporting for other services.
* [**Achievement Service**](https://github.com/CorporationX/achievement_service/tree/basilisk-master-bc4) - Manages and tracks user achievements and milestones.
* [**Notification Service**](https://github.com/CorporationX/notification_service/tree/basilisk-master-bc4) - Handles the delivery of various notifications to users via different channels.
* [**Account Service**](https://github.com/CorporationX/account_service/tree/basilisk-master-bc4) - Manages account information, settings, and related functionalities for users.
* [**Infra**](https://github.com/CorporationX/infra) - Microservices configuration service for developers.

## Features

- **Real-time Notifications** (SMS, Email, Telegram)
- **Infinite-High Available News Feed**
- **User Dashboard Page**
- **Activity Analytics**
- **Cloud Integration**
- **Dual Message Payment System**
- **URL Link Shortener**
- **API Integration**
- **Activity Achievements**
- **CSV File Parcer**

## Technologies Used

- Java, Spring Framework, Kafka, Amazon Web Services (AWS), Docker, Google Cloud Platform (GCP), Kubernetes, Redis,  Amazon S3 Cloud, CI/CD, Hibernate, Multithreading, Liquibase,REST API

## Project Structure

```plaintext
├── .idea  
├── achievement_service/
│   ├── gradle/wrapper/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── README.md
│   ├── build.gradle.kts
│   ├── gradlew
│   ├── gradlew.bat
│   ├── settings.gradle.kts
│   ├── src/
│       ├── main/
│       │   ├── java/
│       │       └── com/
│       │           └── achievement/
│       │               ├── cache/
│       │               ├── client/
│       │               ├── config/
│       │               ├── controller/
│       │               ├── dto/
│       │               ├── event/
│       │               ├── exception/
│       │               ├── filter/
│       │               ├── handler/
│       │               ├── listener/
│       │               ├── mapper/
│       │               ├── model/
│       │               ├── publisher/
│       │               ├── repository/
│       │               ├── service/
│       │               └── AchievementServiceApp.java
│       └── test/
│  
├── analytics_service/
│   ├── gradle/wrapper/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── README.md
│   ├── build.gradle.kts
│   ├── gradlew
│   ├── gradlew.bat
│   ├── settings.gradle.kts
│   └── src/
│       ├── main/
│       │   └── java/
│       │       └── com/
│       │           └── analytics/
│       │               ├── client/
│       │               ├── config/
│       │               ├── controller/
│       │               ├── dto/
│       │               ├── event/
│       │               ├── exception/
│       │               ├── filter/
│       │               ├── handler/
│       │               ├── listener/
│       │               ├── mapper/
│       │               ├── model/
│       │               ├── publisher/
│       │               ├── repository/
│       │               ├── service/
│       │               └── AnalyticsServiceApp.java
│       └── test/
│
├── infra/
│   ├── .gitignore
│   ├── README.md
│   ├── docker-compose.yaml
│   ├── run.sh
│   └── stop.sh
│
├── notification_service/
│   ├── gradle/wrapper/
│   ├── .github/workflows
│   ├── .gitignore
│   ├── Dockerfile
│   ├── README.md
│   ├── build.gradle.kts
│   ├── gradlew
│   ├── gradlew.bat
│   ├── settings.gradle.kts
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── notification/
│   │   │   │           ├── client/
│   │   │   │           ├── config/
│   │   │   │           ├── dto/
│   │   │   │           ├── entity/
│   │   │   │           ├── event/
│   │   │   │           ├── exception/
│   │   │   │           ├── handler/
│   │   │   │           ├── listener/
│   │   │   │           ├── messaging/
│   │   │   │           ├── property/
│   │   │   │           ├── repository/
│   │   │   │           ├── service/
│   │   │   │           └── NotificationServiceApp.java
│   │   ├── test/
│
├── payment_service/
│   ├── gradle/wrapper/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── README.md
│   ├── build.gradle.kts
│   ├── gradlew
│   ├── gradlew.bat
│   ├── settings.gradle.kts
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── payment/
client
config
controller
dto
enums
event
exception
mapper
model
publisher
repository
scheduler
service
validator

│   │   │   │           ├── cache/
│   │   │   │           ├── client/
│   │   │   │           ├── config/
│   │   │   │           ├── controller/
│   │   │   │           ├── dto/
│   │   │   │           ├── event/
│   │   │   │           ├── exception/
│   │   │   │           ├── filter/
│   │   │   │           ├── handler/
│   │   │   │           ├── listener/
│   │   │   │           ├── mapper/
│   │   │   │           ├── model/
│   │   │   │           ├── publisher/
│   │   │   │           ├── repository/
│   │   │   │           ├── service/
│   │   │   │           └── PaymentServiceApp.java
│   │   ├── test/
│
├── post_service/
│   ├── gradle/wrapper/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── README.md
│   ├── build.gradle.kts
│   ├── gradlew
│   ├── gradlew.bat
│   ├── settings.gradle.kts
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── post/

client
config
controller
dto
event
exception
filter
handler
mapper
model
property
publisher
repository
scheduler
service
util
validator
│   │   │   │           ├── cache/
│   │   │   │           ├── client/
│   │   │   │           ├── config/
│   │   │   │           ├── controller/
│   │   │   │           ├── dto/
│   │   │   │           ├── event/
│   │   │   │           ├── exception/
│   │   │   │           ├── filter/
│   │   │   │           ├── handler/
│   │   │   │           ├── listener/
│   │   │   │           ├── mapper/
│   │   │   │           ├── model/
│   │   │   │           ├── publisher/
│   │   │   │           ├── repository/
│   │   │   │           ├── service/
│   │   │   │           └── PostServiceApp.java
│   │   ├── test/
│
├── project_service/
│   ├── gradle/wrapper/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── README.md
│   ├── build.gradle.kts
│   ├── gradlew
│   ├── gradlew.bat
│   ├── settings.gradle.kts
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── project/

client
config
controller
dto
event
exceptions
filter
handler
mapper
model
pattern
property
publisher
repository
service
util
validation

│   │   │   │           ├── cache/
│   │   │   │           ├── client/
│   │   │   │           ├── config/
│   │   │   │           ├── controller/
│   │   │   │           ├── dto/
│   │   │   │           ├── event/
│   │   │   │           ├── exception/
│   │   │   │           ├── filter/
│   │   │   │           ├── handler/
│   │   │   │           ├── listener/
│   │   │   │           ├── mapper/
│   │   │   │           ├── model/
│   │   │   │           ├── publisher/
│   │   │   │           ├── repository/
│   │   │   │           ├── service/
│   │   │   │           └── ProjectServiceApp.java
│   │   ├── test/
│
├── user_service/
│   ├── gradle/wrapper/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── README.md
│   ├── build.gradle.kts
│   ├── gradlew
│   ├── gradlew.bat
│   ├── settings.gradle.kts
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── elevatefi/
│   │   │   │           ├── cache/
│   │   │   │           ├── client/
│   │   │   │           ├── config/
│   │   │   │           ├── controller/
│   │   │   │           ├── dto/
│   │   │   │           ├── event/
│   │   │   │           ├── exception/
│   │   │   │           ├── filter/
│   │   │   │           ├── handler/
│   │   │   │           ├── listener/
│   │   │   │           ├── mapper/
│   │   │   │           ├── model/
│   │   │   │           ├── publisher/
│   │   │   │           ├── repository/
│   │   │   │           ├── service/
│   │   │   │           └── UserServiceApp.java
│   │   ├── test/
│
├── account_service/
│   ├── gradle/wrapper/
│   ├── .gitignore
│   ├── Dockerfile
│   ├── README.md
│   ├── build.gradle.kts
│   ├── gradlew
│   ├── gradlew.bat
│   ├── settings.gradle.kts
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/
│   │   │   │       └── elevatefi/
│   │   │   │           ├── cache/
│   │   │   │           ├── client/
│   │   │   │           ├── config/
│   │   │   │           ├── controller/
│   │   │   │           ├── dto/
│   │   │   │           ├── event/
│   │   │   │           ├── exception/
│   │   │   │           ├── filter/
│   │   │   │           ├── handler/
│   │   │   │           ├── listener/
│   │   │   │           ├── mapper/
│   │   │   │           ├── model/
│   │   │   │           ├── publisher/
│   │   │   │           ├── repository/
│   │   │   │           ├── service/
│   │   │   │           └── UserServiceApp.java
│   │   ├── test/
│
├── .gitignore
├── .gitmodules
├── README.md
├── cherry-pick.sh
├── updated_shell_scripts/
└── push-all.sh
```


