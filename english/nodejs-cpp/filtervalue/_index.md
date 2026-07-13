---
title: FilterValue
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents filter value used in the criteria.
type: docs
url: /nodejs-cpp/filtervalue/
---

## FilterValue class

Represents filter value used in the criteria.

```javascript
class FilterValue;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [stringValue](#stringValue--)| string | Readonly. Gets the string value. |
| [dateTimeGroupItem](#dateTimeGroupItem--)| DateTimeGroupItem | Readonly. Gets date time value. |

## Methods

| Method | Description |
| --- | --- |
| [getStringValue()](#getStringValue--)| <b>@deprecated.</b> Please use the 'stringValue' property instead. Gets the string value. |
| [getDateTimeGroupItem()](#getDateTimeGroupItem--)| <b>@deprecated.</b> Please use the 'dateTimeGroupItem' property instead. Gets date time value. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getValueType()](#getValueType--)| Gets the type of this filter value. |


### stringValue {#stringValue--}

Readonly. Gets the string value.

```javascript
stringValue : string;
```


### dateTimeGroupItem {#dateTimeGroupItem--}

Readonly. Gets date time value.

```javascript
dateTimeGroupItem : DateTimeGroupItem;
```


### getStringValue() {#getStringValue--}

<b>@deprecated.</b> Please use the 'stringValue' property instead. Gets the string value.

```javascript
getStringValue() : string;
```


### getDateTimeGroupItem() {#getDateTimeGroupItem--}

<b>@deprecated.</b> Please use the 'dateTimeGroupItem' property instead. Gets date time value.

```javascript
getDateTimeGroupItem() : DateTimeGroupItem;
```


**Returns**

[DateTimeGroupItem](../datetimegroupitem/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getValueType() {#getValueType--}

Gets the type of this filter value.

```javascript
getValueType() : FilterValueType;
```


**Returns**

[FilterValueType](../filtervaluetype/)


