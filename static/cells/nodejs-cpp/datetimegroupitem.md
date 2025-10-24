##DateTimeGroupItem
Represents the datetimes group setting.
## DateTimeGroupItem class
Represents the datetime's group setting.
```javascript
class DateTimeGroupItem;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Object)](#constructor-object-)| Constructs from an Object convertible to this. |
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
| [getMinValue()](#getMinValue--)| <b>@deprecated.</b> Please use the 'minValue' property instead. Gets the min value. |
| [getDateTimeGroupingType()](#getDateTimeGroupingType--)| <b>@deprecated.</b> Please use the 'dateTimeGroupingType' property instead. Gets and sets the group type. |
| [setDateTimeGroupingType(DateTimeGroupingType)](#setDateTimeGroupingType-datetimegroupingtype-)| <b>@deprecated.</b> Please use the 'dateTimeGroupingType' property instead. Gets and sets the group type. |
| [getYear()](#getYear--)| <b>@deprecated.</b> Please use the 'year' property instead. Gets and sets the year of the grouped date time. |
| [setYear(number)](#setYear-number-)| <b>@deprecated.</b> Please use the 'year' property instead. Gets and sets the year of the grouped date time. |
| [getMonth()](#getMonth--)| <b>@deprecated.</b> Please use the 'month' property instead. Gets and sets the month of the grouped date time. |
| [setMonth(number)](#setMonth-number-)| <b>@deprecated.</b> Please use the 'month' property instead. Gets and sets the month of the grouped date time. |
| [getDay()](#getDay--)| <b>@deprecated.</b> Please use the 'day' property instead. Gets and sets the day of the grouped date time. |
| [setDay(number)](#setDay-number-)| <b>@deprecated.</b> Please use the 'day' property instead. Gets and sets the day of the grouped date time. |
| [getHour()](#getHour--)| <b>@deprecated.</b> Please use the 'hour' property instead. Gets and sets the hour of the grouped date time. |
| [setHour(number)](#setHour-number-)| <b>@deprecated.</b> Please use the 'hour' property instead. Gets and sets the hour of the grouped date time. |
| [getMinute()](#getMinute--)| <b>@deprecated.</b> Please use the 'minute' property instead. Gets and sets the minute of the grouped date time. |
| [setMinute(number)](#setMinute-number-)| <b>@deprecated.</b> Please use the 'minute' property instead. Gets and sets the minute of the grouped date time. |
| [getSecond()](#getSecond--)| <b>@deprecated.</b> Please use the 'second' property instead. Gets and sets the second of the grouped date time. |
| [setSecond(number)](#setSecond-number-)| <b>@deprecated.</b> Please use the 'second' property instead. Gets and sets the second of the grouped date time. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toObject()](#toObject--)| Gets the Object. |
### constructor(Object) {#constructor-object-}
Constructs from an Object convertible to this.
```javascript
constructor(obj: Object);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object. |
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
### getMinValue() {#getMinValue--}
```javascript
getMinValue() : Date;
```
### getDateTimeGroupingType() {#getDateTimeGroupingType--}
```javascript
getDateTimeGroupingType() : DateTimeGroupingType;
```
**Returns**
[DateTimeGroupingType](../datetimegroupingtype/)
### setDateTimeGroupingType(DateTimeGroupingType) {#setDateTimeGroupingType-datetimegroupingtype-}
```javascript
setDateTimeGroupingType(value: DateTimeGroupingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTimeGroupingType](../datetimegroupingtype/) | The value to set. |
### getYear() {#getYear--}
```javascript
getYear() : number;
```
### setYear(number) {#setYear-number-}
```javascript
setYear(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getMonth() {#getMonth--}
```javascript
getMonth() : number;
```
### setMonth(number) {#setMonth-number-}
```javascript
setMonth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getDay() {#getDay--}
```javascript
getDay() : number;
```
### setDay(number) {#setDay-number-}
```javascript
setDay(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHour() {#getHour--}
```javascript
getHour() : number;
```
### setHour(number) {#setHour-number-}
```javascript
setHour(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getMinute() {#getMinute--}
```javascript
getMinute() : number;
```
### setMinute(number) {#setMinute-number-}
```javascript
setMinute(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getSecond() {#getSecond--}
```javascript
getSecond() : number;
```
### setSecond(number) {#setSecond-number-}
```javascript
setSecond(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### toObject() {#toObject--}
Gets the Object.
```javascript
toObject() : Object;
```
