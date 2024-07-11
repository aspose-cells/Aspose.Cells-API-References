---
title: SmartTagPropertyCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all properties of cell smart tag.
type: docs
url: /nodejs-cpp/smarttagpropertycollection/
---

## SmartTagPropertyCollection class

Represents all properties of cell smart tag.

```javascript
class SmartTagPropertyCollection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [SmartTagProperty](./smarttagproperty/) object. |
| [add(string, string)](#add-string-string-)| Adds a property of cell's smart tag. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### get(number) {#get-number-}

Gets a [SmartTagProperty](./smarttagproperty/) object.

```javascript
get(index: number) : SmartTagProperty;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index |

**Returns**

Returns a [SmartTagProperty](./smarttagproperty/) object.

### add(string, string) {#add-string-string-}

Adds a property of cell's smart tag.

```javascript
add(name: string, value: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property |
| value | string | The value of the property. |

**Returns**

return [SmartTagProperty](./smarttagproperty/)

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



