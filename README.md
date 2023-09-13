# Sql_Query_CovidDeaths
# Global Infection Data SQL Queries

## Overview

This repository contains SQL queries to retrieve specific information about the number of people infected with a particular disease worldwide. Additionally, it includes queries that allow users to filter data by country and continent.

## Table of Contents

- [Getting Started](#getting-started)
- [Queries](#queries)
  - [1. Total Global Infections](#1-total-global-infections)
  - [2. Infections by Country](#2-infections-by-country)
  - [3. Infections by Continent](#3-infections-by-continent)
- [Usage](#usage)
- [Contributing](#contributing)


## Getting Started

To use the queries in this repository, you will need access to a database management system (DBMS) that supports SQL queries. Ensure that you have the necessary credentials and connectivity to the database before proceeding.

## Queries

### 1. Total Global Infections

This query retrieves the total number of infections worldwide.

```sql
SELECT SUM(infections) as total_infections
FROM global_infection_data;
```

### 2. Infections by Country

This query allows you to filter the data by country. Replace `'Country Name'` with the desired country's name in single quotes.

```sql
SELECT country_name, infections
FROM global_infection_data
WHERE country_name = 'Country Name';
```

### 3. Infections by Continent

This query allows you to filter the data by continent. Replace `'Continent Name'` with the desired continent's name in single quotes.

```sql
SELECT country_name, continent, infections
FROM global_infection_data
WHERE continent = 'Continent Name';
```

## Usage

1. Copy and paste the desired query into your SQL environment.
2. Replace any placeholders (e.g., 'Country Name' or 'Continent Name') with the specific country or continent you are interested in.
3. Execute the query to obtain the relevant infection data.

## Contributing

If you would like to contribute to this project, please open an issue or submit a pull request. We welcome any suggestions, improvements, or additional queries that could benefit the community.


