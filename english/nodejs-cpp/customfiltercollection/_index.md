---
title: CustomFilterCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the custom filters.
type: docs
url: /nodejs-cpp/customfiltercollection/
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
| [constructor(IObject)](#constructor-iobject-)| Constructs from an IObject convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the custom filter in the specific index. |
| [getAnd()](#getAnd--)| Indicates whether the two criteria have an "and" relationship. |
| [setAnd(boolean)](#setAnd-boolean-)| Indicates whether the two criteria have an "and" relationship. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### constructor() {#constructor--}

Constructs new instance.

```javascript
constructor();
```


### constructor(IObject) {#constructor-iobject-}

Constructs from an IObject convertible to this.

```javascript
constructor(obj: IObject);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | IObject | The object. |

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

### getAnd() {#getAnd--}

Indicates whether the two criteria have an "and" relationship.

```javascript
getAnd() : boolean;
```


### setAnd(boolean) {#setAnd-boolean-}

Indicates whether the two criteria have an "and" relationship.

```javascript
setAnd(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



