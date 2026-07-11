# Scalable Internship Management System

This project implements a scalable internship management database using AWS RDS MySQL.

## Project Overview

The system stores and manages intern application records in a cloud-based MySQL database.

## AWS Services Used

- Amazon RDS for MySQL
- Amazon EC2
- RDS Read Replica
- VPC Security Groups

## Database Details

- Database name: `internship_management`
- Table name: `interns`
- Database engine: MySQL Community
- Primary instance: `database-1`
- Read replica: `database-1-replica`

## Features

- Cloud-hosted MySQL database
- Secure EC2-to-RDS connectivity
- Intern application records management
- Read replica for improved read performance
- SQL queries for record verification

## Table Structure

The `interns` table contains:

- ID
- Full name
- Email
- University
- Department
- Application status

## Sample Operations

- Create database and table
- Insert intern records
- Retrieve all intern records
- Filter names and statuses
- Count total records

## Architecture

```text
EC2 Instance
     |
     v
Primary RDS MySQL
     |
     v
Read Replica
