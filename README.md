Smart Elevator Control

Database Structure : Core Entities

Building → Represents a physical infrastructure unit
Floor → Floors within each building
Elevator_Shaft → Physical shafts holding elevators
Elevator → Elevator units assigned to shafts
Elevator_Floor → Junction table mapping elevators to floors
Floor_Request → Requests generated from floors
Ride → Actual elevator trips (execution of requests)
Maintenance → Maintenance history of elevators

Relationships

One Building → Many Floors

One Building → Many Elevators

One Building → Many Elevator Shafts

One Elevator Shaft → One Elevator

One Elevator ↔ Many Floors 

One Floor → Many Floor Requests

One Floor Request → One Ride

One Elevator → Many Rides

One Elevator → Many Maintenance Records
