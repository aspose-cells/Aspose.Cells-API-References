##VObject
VObject class.
## VObject class
VObject class.
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
| [constructor(bool)](#constructor-bool-)| Constructs from a bool value. |
| [constructor(number)](#constructor-number-)| Constructs from a number value. |
| [constructor(string)](#constructor-string-)| Constructs from a string value. |
| [constructor(Date)](#constructor-date-)| Constructs from a Date value. |
| [constructor(Color)](#constructor-color-)| Constructs from a Color value. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the VObjectType of the vobject. |
| [isBool()](#isBool--)| Checks whether the vobject is a bool value. |
| [isNumber()](#isNumber--)| Checks whether the vobject is a number value. |
| [isNull()](#isNull--)| Checks whether the vobject is null. |
| [isDate()](#isDate--)| Checks whether the vobject is a Date value. |
| [isColor()](#isColor--)| Checks whether the vobject is a Color value. |
| [isString()](#isString--)| Checks whether the vobject is a String value. |
| [isReferredArea()](#isReferredArea--)| Checks whether the vobject is a ReferredArea object. |
| [isRange()](#isRange--)| Checks whether the vobject is a Range object. |
| [isObject()](#isObject--)| Checks whether the vobject is an object pointer. |
| [toBool()](#toBool--)| Gets the bool value. |
| [toNumber()](#toNumber--)| Gets the number value. |
| [toString()](#toString--)| Gets the string value. |
| [toDate()](#toDate--)| Gets the Date value. |
| [toColor()](#toColor--)| Gets the Color value. |
| [toReferredArea()](#toReferredArea--)| Gets the ReferredArea object. |
| [toRange()](#toRange--)| Gets the Range object. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### constructor(bool) {#constructor-bool-}
Constructs from a bool value.
```javascript
constructor(value: boolean);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The bool value. |
### constructor(number) {#constructor-number-}
Constructs from a number value.
```javascript
constructor(value: number);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The number value. |
### constructor(string) {#constructor-string-}
Constructs from a string value.
```javascript
constructor(value: string);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The string value. |
### constructor(Date) {#constructor-date-}
Constructs from a Date value.
```javascript
constructor(value: Date);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The Date value. |
### constructor(Color) {#constructor-color-}
Constructs from a Color value.
```javascript
constructor(value: Color);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Color | The Color value. |
### getType() {#getType--}
Gets the VObjectType of the vobject.
```javascript
getType() : VObjectType;
```
**Returns**
[VObjectType](../objecttype/)
### isBool() {#isBool--}
Checks whether the vobject is a bool value.
```javascript
isBool() : boolean;
```
### isNumber() {#isNumber--}
Checks whether the vobject is a number value.
```javascript
isNumber() : boolean;
```
### isNull() {#isNull--}
Checks whether the vobject is null.
```javascript
isNull() : boolean;
```
### isDate() {#isDate--}
Checks whether the vobject is a Date value.
```javascript
isDate() : boolean;
```
### isColor() {#isColor--}
Checks whether the vobject is a Color value.
```javascript
isColor() : boolean;
```
### isString() {#isString--}
Checks whether the vobject is a String value.
```javascript
isString() : boolean;
```
### isReferredArea() {#isReferredArea--}
Checks whether the vobject is a ReferredArea object.
```javascript
isReferredArea() : boolean;
```
### isRange() {#isRange--}
Checks whether the vobject is a Range object.
```javascript
isRange() : boolean;
```
### isObject() {#isObject--}
Checks whether the vobject is an object pointer.
```javascript
isObject() : boolean;
```
### toBool() {#toBool--}
Gets the bool value.
```javascript
toBool() : boolean;
```
### toNumber() {#toNumber--}
Gets the number value.
```javascript
toNumber() : number;
```
### toString() {#toString--}
Gets the string value.
```javascript
toString() : string;
```
### toDate() {#toDate--}
Gets the Date value.
```javascript
toDate() : Date;
```
### toColor() {#toColor--}
Gets the Color value.
```javascript
toColor() : Color;
```
**Returns**
[Color](../color/)
### toReferredArea() {#toReferredArea--}
Gets the ReferredArea value.
```javascript
toReferredArea() : ReferredArea;
```
**Returns**
[ReferredArea](../referredarea/)
### toRange() {#toRange--}
Gets the Range value.
```javascript
toRange() : Range;
```
**Returns**
[Range](../range/)
