---
title: CustomFilterCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the custom filters.
type: docs
url: /javascript-cpp/customfiltercollection/
---

## CustomFilterCollection class

Represents the custom filters.

```javascript
class CustomFilterCollection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructs new instance. |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [and](#and--)| boolean | Indicates whether the two criteria have an "and" relationship. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the custom filter in the specific index. |
| [custom(FilterOperatorType, VObject, boolean, FilterOperatorType, VObject)](#custom-filteroperatortype-vobject-boolean-filteroperatortype-vobject-)| Filters a list with custom criteria. |
| [toVObject()](#toVObject--)| Gets the VObject. |


### constructor() {#constructor--}

Constructs new instance.

```javascript
constructor();
```


**Remarks**

NOTE: This member is now obsolete. Instead,please set FilterColumn.FilterType as FilterType.CustomFilters then get FilterColumn.CustomFilters. This property will be removed 12 months later since June 2026. Aspose apologizes for any inconvenience you may have experienced.

### constructor(VObject) {#constructor-vobject-}

Constructs from a VObject convertible to this.

```javascript
constructor(vobj: VObject);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vobj | VObject | The vobject. |

### and {#and--}

Indicates whether the two criteria have an "and" relationship.

```javascript
and : boolean;
```


### get(number) {#get-number-}

Gets the custom filter in the specific index.

```javascript
get(index: number) : CustomFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[CustomFilter](../customfilter/)

### custom(FilterOperatorType, VObject, boolean, FilterOperatorType, VObject) {#custom-filteroperatortype-vobject-boolean-filteroperatortype-vobject-}

Filters a list with custom criteria.

```javascript
custom(operatorType1: FilterOperatorType, criteria1: VObject, isAnd: boolean, operatorType2: FilterOperatorType, criteria2: VObject) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| operatorType1 | [FilterOperatorType](../filteroperatortype/) |  |
| criteria1 | VObject |  |
| isAnd | boolean |  |
| operatorType2 | [FilterOperatorType](../filteroperatortype/) |  |
| criteria2 | VObject |  |

### toVObject() {#toVObject--}

Gets the VObject.

```javascript
toVObject() : VObject;
```



