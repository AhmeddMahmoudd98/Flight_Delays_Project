# Flight_Delays_Project
# Overview
This project focuses on analyzing airline flight delays using a structured data model. The model is designed to capture various dimensions and facts related to flight operations, including airport details, carrier information, flight delays, and cancellations. The goal is to provide insights into the factors contributing to flight delays and cancellations, enabling better decision-making and operational improvements.

# Data Model
The data model consists of several dimensions and a fact table, each capturing specific aspects of flight operations:

# Dimensions
# Dim_AirportCodes

airport: Airport identifier.

country_code: Country code of the airport.

 lata: Local Access and Transport Area code.

 region_name: Region or state where the airport is located.

# Dim_Carrier

Carrier Name: Name of the airline carrier.

IATA Carrier Code: IATA code for the carrier.

ICAO Carrier Code: ICAO code for the carrier.

# DateDim

Date: Calendar date.

DateKey: Unique key for the date.

Day: Day of the week.

DayNo: Day number in the month.

Month: Month name.

MonthNo: Month number.

Quarter: Quarter of the year.

Year: Year.

# Dim_Cancelled

CancellationCode: Code indicating the reason for cancellation.

CancellationType: Description of the cancellation reason.

# Fact Table
Fact_DelayedFlights

ActualElapsedTime: Actual elapsed time of the flight.

AirTime: Time spent in the air.

Ar/Delay: Arrival delay.

ARRTime_Formatted: Formatted arrival time.

CancellationCode: Code indicating the reason for cancellation.

Cancelled: Indicates if the flight was cancelled.

CarrierDelay: Delay attributed to the carrier.

CRSArrTime_Formated: Scheduled arrival time.

CRSDepTime_Formated: Scheduled departure time.

CRSElapsedTime: Scheduled elapsed time.

Datekey: Key linking to the DateDim table.

Day: Day of the week.

DayOfWeek: Day of the week (numeric).

DepDelay: Departure delay.

DepTime_formatted: Formatted departure time.

Dest: Destination airport code.

Distance: Distance of the flight.

Diverted: Indicates if the flight was diverted.

FlightNum: Flight number.

ID: Unique identifier for the flight record.
