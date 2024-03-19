In this project, we will develop a Spring Boot application to provide a REST service for the 'GeoHub' application. With the 'GeoHub' application, users can fetch information about cities belonging to specific countries.

For this application, we need to represent two entities: `City` and `Country`. The `City` entity maintains a Many-to-One relationship with the `Country` entity.

Database contains two tables `country` and `city` using the given database schema.

<details>
<summary>**Database Schema**</summary>

#### Country Table

|   Columns   |                 Type                  |
| :---------: | :-----------------------------------: |
|  countryId  | INTEGER (Primary Key, Auto Increment) |
| countryName |                 TEXT                  |
|  currency   |                 TEXT                  |
| population  |                INTEGER                |
|  latitude   |                 TEXT                  |
|  longitude  |                 TEXT                  |

#### City Table

|  Columns   |                 Type                 |
| :--------: | :----------------------------------: |
|   cityId   | INTEGER(Primary Key, Auto Increment) |
|  cityName  |                 TEXT                 |
| population |               INTEGER                |
|  latitude  |                 TEXT                 |
| longitude  |                 TEXT                 |
| countryId  |        INTEGER (Foreign Key)         |

</details>

#### API methods can be executed using platforms like postman.com API management platforms