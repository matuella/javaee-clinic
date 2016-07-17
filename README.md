# JavaEE Clinic
[![Build Status](https://travis-ci.org/matuella/javaee-clinic.svg?branch=master)](https://travis-ci.org/matuella/javaee-clinic)

---
## Introduction
JavaEE project with the purpose of creating a sort of **Clinic Management System**. The system is mainly focused on controlling Appointments, Secretaries, Doctors and Pacients, and with some basic Business rules.

---
## Tools, frameworks and libraries

- Context and Dependency Injection (CDI);
- Enterprise JavaBeans (EJB);
- Java Persistence API (JPA);
- Java Server Faces (JSF);
- Glassfish (Full application server);
- PrimeFaces (JavaEE UI framework);
- Hibernate (ORM and JPA implementation);
- RESTful WebServices (JAX-RS) -> Not implemented yet;
- JUnit -> Not implemented yet;
- JasperReports -> Not implemented yet.

---
## Details about the project

- Singletons to manage some "utilities";
- Focusing on making a UI responsive enough to Desktop/Tablet (you won't manage this kind of stuff on a mobile, right?);
- Filters used to manage the respective users access permissions (and some containers only render for certain users);
- Converters to control some input/outputs, like Dates and Entities;
- Some entities may extend a mapped superclass, like Secretary and Doctor;
- Aiming for something like a modularization of the JSF Pages (mainly the dialogs);
- Hashed the password into the database using PBKDF2 with Salt and HMAC-SHA1;
- Kind of different GenericService without using the DAO layer/pattern.

---
## Running the project...

What you're *probably* going to need (recommended): 
- MySQL (you can easily modify the DB you wanna use in the *persistence.xml*);
- Glassfish 4.1/4.1.1 (or you can use your favorite server that have a *servlet+EJB* container);

#### ...by command line (Maven needed):

To be added...

#### ...using a IDE (NetBeans 8.1 needed):

To be added...

---
## Misc

*"Wait, __without__ the __DAO pattern__?! __Every__ java project  - with persistence - has a DAO layer!!"*

Read the Balazs Zsoldos answer [here](http://stackoverflow.com/questions/3888575/single-dao-generic-crud-methods-jpa-hibernate-spring).
