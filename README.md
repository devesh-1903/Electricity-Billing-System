# Electricity-Billing-System
DESCRIPTION

Electricity Billing System is a desktop based application developed in Java programming language. 
The project aims at serving the department of electricity by computerizing the billing system. 
It mainly focuses on the calculation of Units consumed during the specified time and the money to be paid to electricity offices. 
This computerized system will make the overall billing system easy, accessible, comfortable and effective for consumers.

DATABASE QUERIES
1 - Create database

create database ebs;

2 - use the database you have just created

use ebs;

3 - Create login table

create table login(meter_no varchar(20), username varchar(30), name varchar(30), password varchar(30), user varchar(30));

4 - Create customer table to store information of customers

create table customer(name varchar(30), meter varchar(20), address varchar(50), city varchar(20), state varchar(30), email varchar(30), phone varchar(20));

5 - Create meter_info table to store the meter information of the customer

create table meter_info(meter_number varchar(20), meter_location varchar(20), meter_type varchar(20), phase_code varchar(20), bill_type varchar(20), days varchar(20));

6 - create tax to store the current tax structure

create table tax(cost_per_unit varchar(20), meter_rent varchar(20), service_charge varchar(20), service_tax varchar(20), swacch_bharat_cess varchar(20), fixed_tax varchar(20));

7 - Insert some values in your tax table

insert into tax values('9','47','22','57','6','18');

8 - Create bill table to store the billing information of the customer

create table bill(meter varchar(20), month varchar(20), units varchar(20), total_bill varchar(20), status varchar(20));
