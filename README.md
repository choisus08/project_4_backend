# Flexi Shift- Backend
**Project By:** Susie Gordon


## Descripton
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
    HOME {
        name string 
        position string
        shiftDate string 
        shiftStartTime string 
        shiftEndTime string 
    }
    HOME ||--|{ CREATE : createEntry
    CREATE {
        name string 
        position string
        shiftDate string 
        shiftStartTime string 
        shiftEndTime string 
    }
    HOME ||--|{ EDIT : editEntry
    EDIT {
        name string 
        position string
        shiftDate string 
        shiftStartTime string 
        shiftEndTime string  
    }
    HOME ||--|{ DELETE : deleteEntry
    DELETE {
        name string 
        position string
        shiftDate string 
        shiftStartTime string 
        shiftEndTime string  
    }
```