# ProjectHiveAPI
Documentation of the Project hive API


## Authentication: 

### Header:

``porjecthivetoken`` : It's a series of 32 numbers, randomly generated at your registration. You can access it on your account settings

## Querry Parameters:

### Get events - [GET Method]

------

``userid`` : the id of the user (required)

``datefrom`` : the date  when it's start the records (default: Today)(Format: yyyy-mm-dd)

``privacy`` : the privacy option (0 - public, 1 - private)(optional)

``importance`` : the importance option (0 - default, 1 - important)(optional)

``type`` : if u want to search in the type u can do it (school, private) (optional)

``endpoint``: ``server/geteventdata``

### Get Friends Data - [GET Method]

``userid`` : the id of the user (required)

``endpoint``: ``server/getfriendsdata``

### Delete Events - [DELETE Method]

------
 ``eventid``: eventId (requiered)

``endpoint``: ``server/deleventdata``

### Update Event - [PUT Method]

------
``eventid``: eventid (requiered)

``title``: Title (requiered)

``description``: Description (requiered)

``date``: A date to update the event (yyyy-mm-dd) (requiered)

``privacy``: The privacy (0 - public, 1 - private) (requiered)

``importance``: importance (0 - default, 1 - important) (requiered)

``type``: type (school - private) (requiered)

``endpoing``: ``server/updeventdata``

### Post Events - [POST Method]

------

``userid``: Your user id (requiered)

``title``: Title of the event (requiered)

``description``: Description of the event (requiered)

``date``: The date of the event (yyyy-mm-dd) (requiered) 

``privacy``: Privacy option (0 - public, 1 - private)(optional)

``importance``: Importance option (0 - default, 1 - important)(optional)

``type``: The type of the event (school - private) (optional)

``endpoint``: ``server/posteventdata``
