# Phase 1: Meeting Room Booking — Problem Framing

## 1. Problem

Employees in a company with offices in different cities and countries need to
reserve meeting rooms.

They need a reliable way to find a room that is available at the required
time, has enough capacity, and provides the necessary equipment. The system
should select the employee's current office building by default while still
allowing them to search in another company location. Unclear availability or
room information may lead to wasted time and booking conflicts.

## 2. Goal

Enable an employee to find and reserve a suitable meeting room at their current
office or another selected company location.

## 3. Actors

| Actor | Main responsibility |
| --- | --- |
| Employee | Search, create, view, and cancel their own bookings |
| Administrator | Maintain locations, rooms, and equipment information |

## 4. Example scenario

> Marco searches for a room in the Berlin office for 6 people, on a selected
> date from 10:00 to 16:00 Berlin time, with a TV and whiteboard.

## 5. Main functional requirements

- The system selects the employee's current office building by default.
- The employee can select another company location.
- The employee can select a date and time.
- The employee can enter the number of participants.
- The employee can select required equipment.
- The system shows rooms that are available and satisfy all selected criteria.
- The employee can create, view, and cancel their own future bookings.
- The administrator can manage locations, rooms, and room equipment.

## 6. Business rules

- A booking must have a start time earlier than its end time.
- A room cannot have overlapping confirmed bookings.
- The room capacity must be equal to or greater than the number of participants.
- The room must have all requested equipment in working condition.
- Only active rooms can be booked.
- The employee's current office building is the default search location, but it
  can be changed.
- The location and time zone must be shown before confirmation.

## 7. Non-functional requirements

| Quality | Initial requirement |
| --- | --- |
| Security | Only authenticated company users can access the application. |
| Authorization | Only administrators can manage rooms, locations, and equipment. |
| Reliability | The system must prevent double booking, including simultaneous requests. |
| Performance | Search results should normally appear within two seconds. |
| Usability | An employee should be able to make a basic booking without training. |

## 8. Basic domain model

| Concept | Meaning |
| --- | --- |
| User | An employee or administrator; an employee has a default office location |
| Location | A company office in a particular city, country, and time zone |
| Room | A bookable meeting room belonging to one location |
| Equipment | Equipment belonging to a room, such as a TV or whiteboard |
| Booking | A reservation connecting one user, one room, and one time period |

## 9. MVP scope

### In scope

- One company with multiple locations
- The employee's current office building selected by default
- Room search by location, date, time, capacity, and equipment
- Create, view, and cancel booking
- Basic room and equipment administration
- TV and whiteboard as initial equipment types

### Out of scope

- Recurring bookings
- Outlook or Google Calendar integration
- Catering and visitor management
- Multiple independent companies
