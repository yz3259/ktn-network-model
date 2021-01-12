Header file
===========

id - primary key identifying this train service in the data
unique_identity - composite key identifying the schedule UID and the date the train runs
runs_on - the date the train runs on


Timings file
============

id - primary key identifying this timing point in the data
production_schedule_id - foreign key referencing the 'id' column of the header file
sequence - order in which the timing point appears in the train schedule (0 = first)
location_code - timing point location code (TIPLOC) identifying the location - e.g. EUSTON = London Euston, WATFDJ = Watford Junction
event_type - 'A' for arrival, 'D' for departure
event_time - time that the event is planned to occur
advertised_event_time - time that the event is planned to occur to the public

