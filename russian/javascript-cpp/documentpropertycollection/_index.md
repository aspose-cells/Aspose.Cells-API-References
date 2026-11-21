---
title: DocumentPropertyCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Base class for BuiltInDocumentPropertyCollection..builtindocumentpropertycollection and CustomDocumentPropertyCollection..customdocumentpropertycollection collections.
type: docs
url: /ru/javascript-cpp/documentpropertycollection/
---

## DocumentPropertyCollection class

Base class for [BuiltInDocumentPropertyCollection](../builtindocumentpropertycollection/) and [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) collections.

```javascript
class DocumentPropertyCollection;
```


### Example
```javascript
const { Workbook } = AsposeCells;

//Создайте объект Workbook, вызвав его пустой конструктор
var workbook = new Workbook(data);

//Получите список всех пользовательских свойств документа Excel‑файла
var customProperties = workbook.worksheets.customDocumentProperties;

//Доступ к пользовательскому свойству документа с использованием индекса свойства
var customProperty1 = customProperties.get(3);

//Доступ к пользовательскому свойству документа с использованием имени свойства
var customProperty2 = customProperties.get("rox_Meta1");

console.log("Custom Properties: " + customProperties.count);
```
## Methods

| Method | Description |
| --- | --- |
| [get(string)](#get-string-)| Returns a [DocumentProperty](../documentproperty/) object by the name of the property. |
| [get(number)](#get-number-)| Returns a [DocumentProperty](../documentproperty/) object by index. |
| [contains(string)](#contains-string-)| Returns true if a property with the specified name exists in the collection. |
| [indexOf(string)](#indexOf-string-)| Gets the index of a property by name. |
| [remove(string)](#remove-string-)| Removes a property with the specified name from the collection. |
| [removeAt(number)](#removeAt-number-)| Removes a property at the specified index. |


### get(string) {#get-string-}

Returns a [DocumentProperty](../documentproperty/) object by the name of the property.

```javascript
get(name: string) : DocumentProperty;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The case-insensitive name of the property to retrieve. |

**Returns**

[DocumentProperty](../documentproperty/)

**Remarks**

Returns null if a property with the specified name is not found.

### get(number) {#get-number-}

Returns a [DocumentProperty](../documentproperty/) object by index.

```javascript
get(index: number) : DocumentProperty;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | Zero-based index of the [DocumentProperty](../documentproperty/) to retrieve. |

**Returns**

[DocumentProperty](../documentproperty/)

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


