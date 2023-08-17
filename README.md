ELECTRICITY BILLING AND ANALYSIS SYSTEM

Project Statement :-

Objective :-
   The main objective of our project is to create an admin-user interface for managing electricity consumption data and billing system , where admins can manage data and the users can obtain information about their electricity consumption .

Portals available :

Common portal :-
     Provides option to access admin or user interface

Admin portal :-
    Admins must log in using their credentials and they get access to various options
      Viewing data
      Inserting data
      Updating data
      Deleting data
      Visualise the data (bar graphs)
      User portal :-
      Users must log in with their ID Number and the password assigned to them and can access various options
      Viewing Consumption Data
      Viewing Bill amount along with due date for payment
      Generating a bill



Tables Used :-
  1.Table customer:
    Contains information about users
    Database: electricity
    Creation Code :-
      CREATE TABLE CUSTOMER(
      ID_NUMBER INT(4),
      CUSTOMER_NAME VARCHAR(50),
      ADDRESS VARCHAR(75),
      PHONE_NUMBER CHAR(10));
      Table Data



	
    	
  2.Table current_consumption:
    Contains information about consumption of electricity by customers
    Database: electricity
    Creation Code :-
      CREATE TABLE CURRENT_CONSUMPTION(
      ID_NUMBER CHAR(4),
      PREVIOUS_MONTH_READING CHAR(5),
      PRESENT_MONTH_READING CHAR(5),
      UNITS_CONSUMED CHAR(5));
Table Data



	






  3.Table electricity_bill:
    Contains information about electricity bill to be paid and the due date for payment
    Database: electricity
    Creation Code :-
      CREATE TABLE ELECTRICITY_BILL(
      ID_NUMBER CHAR(4),
      UNITS_CONSUMED CHAR(5),
      RATE_PER_UNIT INT(5),
      BILL_AMOUNT INT(8),
      PERCENTAGE_OF_ADDITIONAL_TAXES FLOAT,
      TOTAL_AMOUNT INT(10),
      DUE_DATE DATE);
    Table Data


