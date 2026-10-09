# Phase 1: Problem Framing


## 1. Problem statement

Answer in two or three sentences:

- Who experiences the problem?
- What are they trying to accomplish?
- What difficulty exists today?
- Why is solving it useful?

**Draft:**

Internal meeting-room booking for one organisation.

## 2. Goal

Describe the outcome the system should enable. Avoid describing a technical
solution.

**Draft:**

Employees need simple way to find available meeting rooms 
and reserve them for specific time. 
The system must prevent conflicting bookings and allow employees to view, edit and cancel their reservations.
Administrators need to maintain room information, manage room availability.

## 3. Actors

For each actor, describe their responsibility and what they need from the
system.

| Actor | Responsibility | Main need |
| Employee | View rooms & add/manage their own bookings | --- |
| Administrator | Has all employees roles & manages rooms and all bookings |  |

## 4. Main use cases

Write short user-focused actions, for example: “View available resources.”

1. View rooms and availability for selected date and time range
2. Booking a space for one person or group of people (select date&time -> system confirms booking)
3. View & cancel own booking
4. Admin - create rooms, edit (name, location, capacity). Change rooms status.
5. Admin - manage all bookings.

## 5. Functional requirements

Describe what the system must do. Use clear, testable statements beginning
with “The system shall...”

- User accesss and permissions 
- Display available rooms for specific date&time range
- Booking creation (date&time validation, prevent overlapping bookings)
- Confirm booking creation
- View & cancel own bookings
- Admin: CRUD rooms & bookings


## 6. Non-functional requirements

Record only requirements that matter to the first slice. Avoid inventing scale
or performance targets without a reason.

| Quality | Requirement | Why it matters |
| --- | --- | --- |
| Security |  |  |
| Reliability |  |  |
| Performance |  |  |
| Usability |  |  |

## 7. Domain model

User {id, name, email, role}
Room {id, name, location, capacity, status}
Booking {id, user_id, room_id, start_time, end_time, status}

