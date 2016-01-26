# Aplikasi Simulator PPOB PLN #

Fitur

* Inquiry
* Payment
* Rekon

## Kebutuhan Software ##

* Git
* MySQL
* Java 1.8
* Maven 3.3


## Cara Setup ##

* Setup Database
* Menjalankan Aplikasi

### Setup Database ###

* Membuat User

    ``` grant all on simulator.* to simulator@localhost identified by 'simulator'; ```

* Membuat Database

    ``` create database simulator; ```

* Bila ada perubahan skema database (file dalam `db/migration)`, database harus didrop dan create ulang

    ``` drop database simulator; create database simulator; ```

### Menjalankan Aplikasi ###

```
mvn clean spring-boot:run
```

Kemudian browse ke `http://localhost:8080`

