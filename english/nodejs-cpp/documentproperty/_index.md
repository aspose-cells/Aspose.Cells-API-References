---
title: DocumentProperty
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a custom or builtin document property.
type: docs
url: /nodejs-cpp/documentproperty/
---

## DocumentProperty class

Represents a custom or built-in document property.

```javascript
class DocumentProperty;
```


### Example
```javascript
const { Workbook } = require("aspose.cells.node");

//Instantiate a Workbook object
var workbook = new Workbook("input/CustomProperties.xlsx");
//Retrieve a list of all custom document properties of the Excel file
var customProperties = workbook.getWorksheets().getCustomDocumentProperties();
//Accessng a custom document property by using the property index
var customProperty1 = customProperties.get(3);
//Accessng a custom document property by using the property name
var customProperty2 = customProperties.get("Owner");
```
## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| Returns the name of the property. |
| [getValue()](#getValue--)| Gets or sets the value of the property. |
| [setValue(Object)](#setValue-object-)| Gets or sets the value of the property. |
| [isLinkedToContent()](#isLinkedToContent--)| Indicates whether this property is linked to content |
| [getSource()](#getSource--)| The linked content source. |
| [getType()](#getType--)| Gets the data type of the property. |
| [isGeneratedName()](#isGeneratedName--)| Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
| [toString()](#toString--)| Returns the property value as a string. |
| [toInt()](#toInt--)| Returns the property value as integer. |
| [toDouble()](#toDouble--)| Returns the property value as double. |
| [toDateTime()](#toDateTime--)| Returns the property value as DateTime in local timezone. |
| [toBool()](#toBool--)| Returns the property value as bool. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getName() {#getName--}

Returns the name of the property.

```javascript
getName() : string;
```


### getValue() {#getValue--}

Gets or sets the value of the property.

```javascript
getValue() : Object;
```


### setValue(Object) {#setValue-object-}

Gets or sets the value of the property.

```javascript
setValue(value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |

### isLinkedToContent() {#isLinkedToContent--}

Indicates whether this property is linked to content

```javascript
isLinkedToContent() : boolean;
```


### getSource() {#getSource--}

The linked content source.

```javascript
getSource() : string;
```


### getType() {#getType--}

Gets the data type of the property.

```javascript
getType() : PropertyType;
```


**Returns**

[PropertyType](../propertytype/)

### isGeneratedName() {#isGeneratedName--}

Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API.

```javascript
isGeneratedName() : boolean;
```


### toString() {#toString--}

Returns the property value as a string.

```javascript
toString() : string;
```


**Remarks**

Converts a number property using Object.ToString(). Converts a boolean property into "Y" or "N". Converts a date property into a short date string.

### toInt() {#toInt--}

Returns the property value as integer.

```javascript
toInt() : number;
```


**Remarks**

Throws an exception if the property type is not PropertyType.Number.

### toDouble() {#toDouble--}

Returns the property value as double.

```javascript
toDouble() : number;
```


**Remarks**

Throws an exception if the property type is not PropertyType.Float.

### toDateTime() {#toDateTime--}

Returns the property value as DateTime in local timezone.

```javascript
toDateTime() : Date;
```


**Remarks**

Throws an exception if the property type is not PropertyType.Date.

### toBool() {#toBool--}

Returns the property value as bool.

```javascript
toBool() : boolean;
```


**Remarks**

Throws an exception if the property type is not PropertyType.Boolean.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



