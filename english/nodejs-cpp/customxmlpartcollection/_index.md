---
title: CustomXmlPartCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a Custom XML Data Storage Part custom XML data within a package.
type: docs
url: /nodejs-cpp/customxmlpartcollection/
---

## CustomXmlPartCollection class

Represents a Custom XML Data Storage Part (custom XML data within a package).

```javascript
class CustomXmlPartCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets an item at the specified index. |
| [add(number[], number[])](#add-numberarray-numberarray-)| Adds an item to the collection. |
| [selectByID(string)](#selectByID-string-)| Gets an item by id. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets an item at the specified index.

```javascript
get(index: number) : CustomXmlPart;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[CustomXmlPart](../customxmlpart/)

### add(number[], number[]) {#add-numberarray-numberarray-}

Adds an item to the collection.

```javascript
add(data: number[], shemaData: number[]) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | number[] | The XML content of this Custom XML Data Storage Part. |
| shemaData | number[] | The set of XML schemas that are associated with this custom XML part. |

### selectByID(string) {#selectByID-string-}

Gets an item by id.

```javascript
selectByID(id: string) : CustomXmlPart;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| id | string | Contains the GUID for the custom XML part. |

**Returns**

[CustomXmlPart](../customxmlpart/)

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



