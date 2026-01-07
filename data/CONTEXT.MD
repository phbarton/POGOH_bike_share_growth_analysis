# CONTEXT+DATASET - POGOH Bike Share Growth Analysis

## Project Type

This is a **Decision Support Project** focused on operational analysis and growth optimization for Pittsburgh's bike share system.

## Background

POGOH (Pittsburgh On the GO, Healthy) is Pittsburgh's nonprofit bike share system. For organizational background and history, see: https://pogoh.com/about-us/

## Motivation

POGOH is experiencing growth, but leadership lacks granular insights into the patterns and drivers of this growth. Current reporting provides only high-level metrics without revealing the underlying dynamics that could inform strategic decisions.

## Objective

Analyze POGOH trip data to answer key questions about growth patterns:
- What is the shape of the growth? 
- Which stations are driving growth?
- Are particular times of day or seasons showing growth?
- How has the introduction of e-bikes affected growth patterns?
- How have changes in pricing and membership structures impacted usage?
- What opportunities exist for continued growth?

## Success Criteria

Generate actionable insights that identify specific opportunities for growth, such as:
- Optimal locations for new stations
- New membership models or pricing strategies
- Reallocation of bikes or resources
- Operational improvements

## Deliverable

A comprehensive analysis report with executive presentation summarizing key findings, growth patterns, and strategic recommendations.

## Role

You are a data analyst intern from a local university working with the Director of Operations on a summer project to understand system growth.

## Stakeholders

- **Executive Director**: Overall strategic vision and organizational leadership
- **Director of Marketing and Outreach**: Customer acquisition and community engagement
- **Director of Operations**: Day-to-day system management and optimization
- **Operations Staff**: Station maintenance and bike redistribution
- **Board of Directors**: Governance and major strategic decisions

---

# DATASETS

## Data Source Description

The POGOH trip dataset contains records of all bike share trips from system launch (2015 as Healthy Ride) through present operations. Each record represents a single trip with information about timing, stations, user type, and bike type.

## Provenance

Trip data is automatically collected by the bike share system when users check out and return bikes. Data has been anonymized to remove personally identifiable information.

## Data Source

Data provided directly by POGOH from their operational database.

## Data Dictionary

**Key Fields:**
- `Id`: Unique trip identifier
- `Closed Status`: Trip completion status (NORMAL, GRACE_PERIOD)
- `Duration`: Trip length in seconds
- `Start Station Id` & `Start Station Name`: Origin station
- `Start Date` & `End Date`: Trip timestamps
- `End Station Id` & `End Station Name`: Destination station
- `acct ID` - Anonymized rider identifier
- `Rider Type`: MEMBER or CASUAL
- `Bike Model`: FIT (traditional) or EFIT (e-bike)
- `Product Name`: Membership type used

Additional station information (locations, capacity, neighborhoods) available separately.

## Data Quality Notes

- Some very short trips may represent bike testing rather than actual usage
- Early years may have different data quality as system evolved
- 2022 represents major system transition from Healthy Ride to POGOH

## Ethical Considerations

While data is anonymized, avoid analysis that could identify individuals through trip patterns. Consider equity implications when making recommendations about station placement or pricing changes.