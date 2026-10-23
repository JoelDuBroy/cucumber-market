# :file_folder: cucumber-market
- A toy project to develop the second-hand goods trading platform Oi Market, similar to Danggeun Market and Bungae Mart.
- The web UI was replaced with Kakao Oven, so the frontend was omitted to focus development on the backend.

## :pushpin: Development Focus
- Aim to implement code with consideration for **reusability** and **maintainability**, not just simple feature implementation.
- Develop with consideration for actual **collaboration with the frontend**, rather than relying on the server-side rendering techniques learned so far.
- Follow the fundamental object-oriented principles **DIP** and **OCP** for **scalability**.
- Utilize Spring Framework's **IoC/DI** and **AOP**.
- Make reasoned choices when adding libraries or features, with consideration for their **purpose of use**.
- Use **JSON** in key-value format for all data communication.
- Choose **RuntimeException** handling and consider the appropriate **HTTP status** for each error type.
- Implement login functionality with **high-traffic load** in mind.
- Design meaningful domains with resource awareness - **Restful API**.
- Set up **MySQL query routing (Replication)** and **Redis Master-Slave** environment for **load balancing and fault tolerance**.
- Build a **multi-server environment** and establish the corresponding **CI/CD** pipeline.

## :wrench: Tech Stack

| Category | Content |
| --- | --- |
| **Language** | Java 11 |
| **Framework** | Spring Boot 2.5.7 |
| **RDBMS** | MySQL 8.0.x |
| **SQL Mapper** | Mybatis |
| **Session Server** | Redis |
| **Web Server** | Nginx |
| **CI/CD** | Jenkins |
| **Container** | Docker |
| **Build Tool** | Gradle 7.3 |
| **API Documentation** | Springfox OpenAPI 3.0 |
| **Boilerplate Code Library** | Lombok |
| **IDE** | IntelliJ IDEA |

## :tv: Web Application UI
:point_right: [**cucumber-market Prototype UI Kakao Oven link**](https://ovenapp.io/view/nlfjeRbawILO48ugsXrRsyt6UI2Bdusk/)

**:point_down: Preview**
<img src = "https://user-images.githubusercontent.com/86584999/145708688-c8295288-df79-48e0-a125-9b855bc4f560.PNG" width="90%" height="45%">
<img src = "https://user-images.githubusercontent.com/86584999/145706256-0811c927-a8e4-45b1-8071-cc0b61496879.PNG" width="90%" height="45%">

## :clapper: Architecture
:point_right: [**Full architecture link**](https://github.com/Hwangwonuk/cucumber-market/wiki/Architecture)
:point_right: [**MySQL architecture link**](https://github.com/Hwangwonuk/cucumber-market/wiki/MySQL-Architecture)
:point_right: [**Redis architecture link**](https://github.com/Hwangwonuk/cucumber-market/wiki/Redis-Architecture)

- **Architecture**
![Architecture](https://user-images.githubusercontent.com/86584999/148683016-53b8e2e7-c577-4e20-9d67-a8d586e7e6cd.jpg)

## :books: Layer
<img src = "https://user-images.githubusercontent.com/86584999/145710572-9df24562-2fd7-45fe-98b7-6345a6aaac34.png">

## :floppy_disk: ERD
:point_right: [**View details**](https://github.com/Hwangwonuk/cucumber-market/wiki/ERD)

<img src = "https://user-images.githubusercontent.com/86584999/145718047-cef57cfa-e28e-40e8-80c3-f92923320a27.png">

## :page_with_curl: Springfox OpenAPI 3.0
**:point_down: Springfox (Swagger) preview**

<img src = "https://user-images.githubusercontent.com/86584999/145809566-f0551828-60de-45cc-9fde-f41e79e3d7f2.JPG">
<img src = "https://user-images.githubusercontent.com/86584999/145809586-bcd7cdc8-4e8b-434c-9768-9260238c058d.JPG">
<img src = "https://user-images.githubusercontent.com/86584999/145809600-3383f9c6-7d95-41df-be8b-c69ca4678472.JPG">

## :computer: Main Features
:point_right: [**Business logic for each feature**](https://github.com/Hwangwonuk/cucumber-market/wiki/Business-Rule)
:point_right: [**Use cases for each feature**](https://github.com/Hwangwonuk/cucumber-market/wiki/Use-Case)

: b usts_in_silhouette: **Users**
- Sign up, withdraw
- Log in, log out
- My page, update profile information
- Register, edit, and delete items for sale
- Product search
- Wishlist feature
- 1:1 chat using secret comments

:guardsman: **Admin**
- View all members
- Register existing members as admins
- Category management

## :warning: Issues Faced During the Project and Lessons Learned
* [**Project learning notes** personal blog](https://wonuk.tistory.com/category/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EA%B4%80%EB%A0%A8)
* [**MultipartFile binding issue** Pull Request](https://github.com/Hwangwonuk/cucumber-market/pull/19)
* [**ArgumentResolver and Springfox conflict issue** Pull Request](https://github.com/Hwangwonuk/cucumber-market/pull/10)
* [**DTO JSON data parsing issue using Lombok** Pull Request](https://github.com/Hwangwonuk/cucumber-market/pull/6)
* [**Spring Boot and Springfox version compatibility issue** wiki](https://github.com/Hwangwonuk/cucumber-market/wiki/Spring-Boot%EC%99%80-Springfox-%EB%B2%84%EC%A0%84-%ED%98%B8%ED%99%98-%EC%9D%B4%EC%8A%88)
* [**Test code JSON parsing error** Issue](https://github.com/Hwangwonuk/cucumber-market/issues/30)
* [**Issue where body is recognized as null when running test code** Issue](https://github.com/Hwangwonuk/cucumber-market/issues/28)
* [**Response to logback library vulnerability** Issue](https://github.com/Hwangwonuk/cucumber-market/issues/26)
