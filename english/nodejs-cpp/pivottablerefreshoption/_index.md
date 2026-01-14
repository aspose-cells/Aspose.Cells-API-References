---
title: PivotTableRefreshOption
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of refreshing data source of the pivot table.
type: docs
url: /nodejs-cpp/pivottablerefreshoption/
---

## PivotTableRefreshOption class

Represents the options of refreshing data source of the pivot table.

```javascript
class PivotTableRefreshOption;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Represents the options of refreshing data source of the pivot table. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [reserveMissingPivotItemType](#reserveMissingPivotItemType--)| ReserveMissingPivotItemType | Represents how to reserve missing pivot items. |
| [isKeepOriginalOrder](#isKeepOriginalOrder--)| boolean | Indicates whether to keep pivot items' original order as old data source. |

## Methods

| Method | Description |
| --- | --- |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--)| <b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items. |
| [setReserveMissingPivotItemType(ReserveMissingPivotItemType)](#setReserveMissingPivotItemType-reservemissingpivotitemtype-)| <b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items. |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--)| <b>@deprecated.</b> Please use the 'isKeepOriginalOrder' property instead. Indicates whether to keep pivot items' original order as old data source. |
| [setIsKeepOriginalOrder(boolean)](#setIsKeepOriginalOrder-boolean-)| <b>@deprecated.</b> Please use the 'isKeepOriginalOrder' property instead. Indicates whether to keep pivot items' original order as old data source. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Represents the options of refreshing data source of the pivot table.

```javascript
constructor();
```


### reserveMissingPivotItemType {#reserveMissingPivotItemType--}

Represents how to reserve missing pivot items.

```javascript
reserveMissingPivotItemType : ReserveMissingPivotItemType;
```


### isKeepOriginalOrder {#isKeepOriginalOrder--}

Indicates whether to keep pivot items' original order as old data source.

```javascript
isKeepOriginalOrder : boolean;
```


**Remarks**

Only applicable for the pivot field which is not sorted. When refreshing such kind of pivot field, Ms Excel keeps the original order of old data source. Default value of this property is true, representing the same behavior with Ms Excel. If user needs the pivot field to be refreshed completely as the data in the new data source, this property should be set as false.

### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}

<b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items.

```javascript
getReserveMissingPivotItemType() : ReserveMissingPivotItemType;
```


**Returns**

[ReserveMissingPivotItemType](../reservemissingpivotitemtype/)

### setReserveMissingPivotItemType(ReserveMissingPivotItemType) {#setReserveMissingPivotItemType-reservemissingpivotitemtype-}

<b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items.

```javascript
setReserveMissingPivotItemType(value: ReserveMissingPivotItemType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ReserveMissingPivotItemType](../reservemissingpivotitemtype/) | The value to set. |

### isKeepOriginalOrder() {#isKeepOriginalOrder--}

<b>@deprecated.</b> Please use the 'isKeepOriginalOrder' property instead. Indicates whether to keep pivot items' original order as old data source.

```javascript
isKeepOriginalOrder() : boolean;
```


**Remarks**

Only applicable for the pivot field which is not sorted. When refreshing such kind of pivot field, Ms Excel keeps the original order of old data source. Default value of this property is true, representing the same behavior with Ms Excel. If user needs the pivot field to be refreshed completely as the data in the new data source, this property should be set as false.

### setIsKeepOriginalOrder(boolean) {#setIsKeepOriginalOrder-boolean-}

<b>@deprecated.</b> Please use the 'isKeepOriginalOrder' property instead. Indicates whether to keep pivot items' original order as old data source.

```javascript
setIsKeepOriginalOrder(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only applicable for the pivot field which is not sorted. When refreshing such kind of pivot field, Ms Excel keeps the original order of old data source. Default value of this property is true, representing the same behavior with Ms Excel. If user needs the pivot field to be refreshed completely as the data in the new data source, this property should be set as false.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



