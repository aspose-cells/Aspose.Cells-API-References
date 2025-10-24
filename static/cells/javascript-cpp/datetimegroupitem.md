##DateTimeGroupItem
Represents the datetimes group setting.
## DateTimeGroupItem class
Represents the datetime's group setting.
```javascript
class DateTimeGroupItem;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |
| [constructor(DateTimeGroupingType, number, number, number, number, number, number)](#constructor-datetimegroupingtype-number-number-number-number-number-number-)|  |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [minValue](#minValue--)| Date | Readonly. Gets the min value. |
| [dateTimeGroupingType](#dateTimeGroupingType--)| DateTimeGroupingType | Gets and sets the group type. |
| [year](#year--)| number | Gets and sets the year of the grouped date time. |
| [month](#month--)| number | Gets and sets the month of the grouped date time. |
| [day](#day--)| number | Gets and sets the day of the grouped date time. |
| [hour](#hour--)| number | Gets and sets the hour of the grouped date time. |
| [minute](#minute--)| number | Gets and sets the minute of the grouped date time. |
| [second](#second--)| number | Gets and sets the second of the grouped date time. |
## Methods
| Method | Description |
| --- | --- |
| [toVObject()](#toVObject--)| Gets the VObject. |
### constructor(VObject) {#constructor-vobject-}
Constructs from a VObject convertible to this.
```javascript
constructor(vobj: VObject);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vobj | VObject | The vobject. |
### constructor(DateTimeGroupingType, number, number, number, number, number, number) {#constructor-datetimegroupingtype-number-number-number-number-number-number-}
```javascript
constructor(type: DateTimeGroupingType, year: number, month: number, day: number, hour: number, minute: number, second: number);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [DateTimeGroupingType](../datetimegroupingtype/) |  |
| year | number |  |
| month | number |  |
| day | number |  |
| hour | number |  |
| minute | number |  |
| second | number |  |
### minValue {#minValue--}
Readonly. Gets the min value.
```javascript
minValue : Date;
```
### dateTimeGroupingType {#dateTimeGroupingType--}
Gets and sets the group type.
```javascript
dateTimeGroupingType : DateTimeGroupingType;
```
### year {#year--}
Gets and sets the year of the grouped date time.
```javascript
year : number;
```
### month {#month--}
Gets and sets the month of the grouped date time.
```javascript
month : number;
```
### day {#day--}
Gets and sets the day of the grouped date time.
```javascript
day : number;
```
### hour {#hour--}
Gets and sets the hour of the grouped date time.
```javascript
hour : number;
```
### minute {#minute--}
Gets and sets the minute of the grouped date time.
```javascript
minute : number;
```
### second {#second--}
Gets and sets the second of the grouped date time.
```javascript
second : number;
```
### toVObject() {#toVObject--}
Gets the VObject.
```javascript
toVObject() : VObject;
```
