---
title: CustomPropertyCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: A collection of CustomPropertynodejscppcustomproperty objects that represent additional information.
type: docs
url: /nodejs-cpp/custompropertycollection/
---

## CustomPropertyCollection class

A collection of [CustomProperty](/nodejs-cpp/customproperty/) objects that represent additional information.

```javascript
class CustomPropertyCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the custom property by the specific index. |
| [add(string, string)](#add-string-string-)| Adds custom property information. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the custom property by the specific index.

```javascript
get(index: number) : CustomProperty;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

The custom property

### add(string, string) {#add-string-string-}

Adds custom property information.

```javascript
add(name: string, value: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the custom property. |
| value | string | The value of the custom property. |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



