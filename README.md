# LA_Metro_Bike

The Metro Bike Share system makes bikes available 24/7, 365 days a year in Downtown LA, Central LA, North Hollywood and the Westside. Metro Bike Share offers convenient round-the-clock access to a fleet of bicycles for short trips. Metro Bike Share is one of LA Metro's multiple public transportation options for Angelenos and visitors to get around.


Metro Bike Share is a partnership between Metro and the City of Los Angeles.

Metro is a multimodal transportation agency that is really three companies in one: a major operator that transports about 1.5 million boarding passengers on an average weekday on a fleet of 2,200 clean air buses and six rail lines, a major construction agency that oversees many bus, rail, highway and other mobility-related building projects, and it is the lead transportation planning and programming agency for Los Angeles County.  

Data Format
Each .csv file contains data for one quarter of the year. Each file contains the following data points:

trip_id: Locally unique integer that identifies the trip
duration: Length of trip in minutes (it is actually in seconds once I cleaned table)
start_time: The date/time when the trip began, presented in ISO 8601 format in local time
end_time: The date/time when the trip ended, presented in ISO 8601 format in local time
start_station: The station ID where the trip originated (for station name and more information on each station see the Station Table)
start_lat: The latitude of the station where the trip originated
start_lon: The longitude of the station where the trip originated
end_station: The station ID where the trip terminated (for station name and more information on each station see the Station Table)
end_lat: The latitude of the station where the trip terminated
end_lon: The longitude of the station where the trip terminated
bike_id:  Locally unique integer that identifies the bike
plan_duration: The number of days that the plan the passholder is using entitles them to ride; 0 is used for a single ride plan (Walk-up)
trip_route_category: "Round Trip" for trips starting and ending at the same station or "One Way" for all other trips
passholder_type: The name of the passholder's plan
bike_type: The kind of bike used on the trip, including standard pedal-powered bikes, electric assist bikes, or smart bikes.


Station Information

Data Format
Station ID: Unique integer that identifies the station (this is the same ID used in the Trips and Station Status data)
Station Name: The public name of the station. "Virtual Station" is used by staff to check in or check out a bike remotely for a special event or in a situation in which a bike could not otherwise be checked in or out to a station.
Go live date: The date that the station was first available
Region: The municipality or area where a station is located, includes DTLA (Downtown LA), Pasadena, Port of LA, Venice
Status: "Active" for stations available or "Inactive" for stations that are not available as of the latest update

Source: 2017 Annual Trips & Stations Datasets https://bikeshare.metro.net/about/data/
