# Rides dashboard

A small public dashboard of daily ride activity for a handful of cities, used to compare how riding varies across cities and across the week.

## Language

### Ride activity

**City**:
A place whose ride activity the dashboard reports, such as Boston, Denver or Miami.
_Avoid_: Market, region, location

**Ride count**:
The number of rides recorded in one City on one Date.
_Avoid_: Trips, volume, ride total (for a single day)

**Date**:
The calendar day on which a Ride count was recorded, as written in the data, independent of any viewer's time zone.
_Avoid_: Timestamp, day (when the calendar day is meant)

### Day types

**Day type**:
The class a Date falls into: either Weekday or Weekend.
_Avoid_: Day category, day kind

**Weekend**:
A Date that is a Saturday or a Sunday.
_Avoid_: Non-working day, holiday

**Weekday**:
A Date that is Monday through Friday, including public holidays that fall on those days.
_Avoid_: Workday, business day

**Average rides per day**:
For one City and one Day type, the sum of its Ride counts divided by the number of Dates of that Day type with a Ride count for that City. A City with no such Dates has no Average rides per day for that Day type, which is not the same as an average of zero.
_Avoid_: Ride totals, daily average (unqualified), mean rides
