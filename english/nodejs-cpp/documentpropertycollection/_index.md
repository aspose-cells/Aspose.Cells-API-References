---
title: DocumentPropertyCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Base class for [BuiltInDocumentPropertyCollection](./builtindocumentpropertycollection/) and [BuiltInDocumentPropertyCollection](./builtindocumentpropertycollection/) collections.
type: docs
url: /nodejs-cpp/documentpropertycollection/
---

## DocumentPropertyCollection class

Base class for [BuiltInDocumentPropertyCollection](./builtindocumentpropertycollection/) and [BuiltInDocumentPropertyCollection](./builtindocumentpropertycollection/) collections.

```javascript
class DocumentPropertyCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [contains(string)](#contains-string-)| Returns true if a property with the specified name exists in the collection. |
| [indexOf(string)](#indexOf-string-)| Gets the index of a property by name. |
| [remove(string)](#remove-string-)| Removes a property with the specified name from the collection. |
| [removeAt(number)](#removeAt-number-)| Removes a property at the specified index. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [get(string)](#get-string-)| Returns a [DocumentProperty](./documentproperty/) object by the name of the property. |


### contains(string) {#contains-string-}

Returns true if a property with the specified name exists in the collection.

```javascript
contains(name: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |

**Returns**

True if the property exists in the collection; false otherwise.

### indexOf(string) {#indexOf-string-}

Gets the index of a property by name.

```javascript
indexOf(name: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |

**Returns**

The zero based index. Negative value if not found.

### remove(string) {#remove-string-}

Removes a property with the specified name from the collection.

```javascript
remove(name: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property. |

### removeAt(number) {#removeAt-number-}

Removes a property at the specified index.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index. |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```


### get(string) {#get-string-}

Returns a [DocumentProperty](./documentproperty/) object by the name of the property.

```javascript
get(name: string) : DocumentProperty;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property to retrieve. |

**Returns**

[DocumentProperty](./documentproperty/)

**Remarks**

<p>Returns null if a property with the specified name is not found.</p>


