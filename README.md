# Flexi Shift- Backend
**Project By:** Susie Gordon


## Descripton
Flexi Shift is an app that conveniently helps employers and employees schedule individual work shifts. Users can view their manually added list of shifts and the calendar month of choice displaying all other reserved shifts added by supervisors, colleagues, or coworkers. 
</br>

## Link
[**Deployment**](DEPLOYMENT LINK)
</br>

## Technologies Used
- Django
- Postman
- Python
</br>

## Backend Endpoints

| Name | ENDPOINT | METHOD | PURPOSE |
|------|----------|--------|---------|
|INDEX| /shift | GET | return list of shift entries|
|DESTROY| /shift/:id | DELETE | delete a shift entry from database |
|UPDATE| /shift/:id | PUT | receive info & update shift entry in database |
|CREATE| /shift | POST | receive info from new form & create new shift entry in database |
|SHOW| /shift/:id | GET | render page with the shift entry|
</br>

## ERD

``` mermaid
erDiagram
    USER {
        username string 
        password string
    }
    USER ||--|{ SHIFTS : Create
    SHIFTS {
        Name string 
        Position string
        Date string 
        ShiftStartTime string 
        ShiftEndTime string 
    }
```