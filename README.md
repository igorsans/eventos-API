# API events

## EndPoints

### Events

* Get /api/event

 ```
[
    {
        "id": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxx",
        "title": "Event Name",
        "description": "Event Description",
        "date": "2065-08-21T02:02:00.999+00:00",
        "city": "Event City",
        "state": "Uf Event",
        "remote": false,
        "eventUrl": "https://event.com.br/"
    },
    {...other events}
]
 ```

* Get by event Id, /api/event/{eventId}


```
[
   {
       "id": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxx",
       "title": "Event Name",
       "description": "Event Description",
       "date": "2065-08-21T02:02:00.999+00:00",
       "city": "Event City",
       "state": "Uf Event",
       "remote": false,
       "eventUrl": "https://event.com.br/"
   }
]
Use this EndPoint to search one event specifically.
```

* Get events with pagination, /api/event?page=0&size=10

```
You can return a capacity determined by you.
```

* Get events with Filters, /api/event/filter?
```
You can search a event by title, city, uf, startDate, endDate
```

* Post event, /api/event
```
{
    "title" : "Event name",
    "description" : "Event Description",
    "eventUrl" : "https://event.com.br/",
    "image" : "",
    "date" : 3018045720999,
    "remote" : false,
    "city" : "City name",
    "state": "UF"
}
```
### Coupon
* Post coupon, /api/coupon/{event ID}
```
{
"code": 123456,
"discout" : 25,
"valid" : null,
}
```