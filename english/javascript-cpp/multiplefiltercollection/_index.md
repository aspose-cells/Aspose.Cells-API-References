---
title: MultipleFilterCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the multiple filter collection.
type: docs
url: /javascript-cpp/multiplefiltercollection/
---

## MultipleFilterCollection class

Represents the multiple filter collection.

```javascript
class MultipleFilterCollection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructs one new instance. |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [matchBlank](#matchBlank--)| boolean | Indicates whether to filter by blank. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [DateTimeGroupItem](../datetimegroupitem/) or a string value. |
| [add(string)](#add-string-)| Adds a label filter criteria. |
| [add(DateTimeGroupingType, number, number, number)](#add-datetimegroupingtype-number-number-number-)| Adds a date filter criteria value. |
| [add(DateTimeGroupingType, number, number, number, number, number, number)](#add-datetimegroupingtype-number-number-number-number-number-number-)| Adds a date time filter criteria value. |
| [toVObject()](#toVObject--)| Gets the VObject. |


### constructor() {#constructor--}

Constructs one new instance.

```javascript
constructor();
```


### constructor(VObject) {#constructor-vobject-}

Constructs from a VObject convertible to this.

```javascript
constructor(vobj: VObject);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vobj | VObject | The vobject. |

### matchBlank {#matchBlank--}

Indicates whether to filter by blank.

```javascript
matchBlank : boolean;
```


### get(number) {#get-number-}

Gets [DateTimeGroupItem](../datetimegroupitem/) or a string value.

```javascript
get(index: number) : VObject;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### add(string) {#add-string-}

Adds a label filter criteria.

```javascript
add(filter: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filter | string | The filter data. |

### add(DateTimeGroupingType, number, number, number) {#add-datetimegroupingtype-number-number-number-}

Adds a date filter criteria value.

```javascript
add(type: DateTimeGroupingType, year: number, month: number, day: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [DateTimeGroupingType](../datetimegroupingtype/) | The type of date filter. |
| year | number | The year. |
| month | number | The month. |
| day | number | The day. |

### add(DateTimeGroupingType, number, number, number, number, number, number) {#add-datetimegroupingtype-number-number-number-number-number-number-}

Adds a date time filter criteria value.

```javascript
add(type: DateTimeGroupingType, year: number, month: number, day: number, hour: number, minute: number, second: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [DateTimeGroupingType](../datetimegroupingtype/) | The type of date filter. |
| year | number | The year. |
| month | number | The month. |
| day | number | The day. |
| hour | number | The hour. |
| minute | number | The minute. |
| second | number | The second. |

### toVObject() {#toVObject--}

Gets the VObject.

```javascript
toVObject() : VObject;
```



