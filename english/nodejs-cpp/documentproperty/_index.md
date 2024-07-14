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


## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| Returns the name of the property. |
| [isLinkedToContent()](#isLinkedToContent--)| Indicates whether this property is linked to content |
| [getSource()](#getSource--)| The linked content source. |
| [getType()](#getType--)| Gets the data type of the property. |
| [isGeneratedName()](#isGeneratedName--)| Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
| [toString()](#toString--)| Returns the property value as a string. |
| [toInt()](#toInt--)| Returns the property value as integer. |
| [toDouble()](#toDouble--)| Returns the property value as double. |
| [toDateTime()](#toDateTime--)| Returns the property value as DateTime in local timezone. |
| [toBool()](#toBool--)| Returns the property value as bool. |


### getName() {#getName--}

Returns the name of the property.

```javascript
getName() : string;
```


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

[PropertyType](/nodejs-cpp/propertytype/)

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

<p>Converts a number property using Object.ToString(). Converts a boolean property into "Y" or "N". Converts a date property into a short date string.</p>

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

<p>Throws an exception if the property type is not PropertyType.Date.</p>

### toBool() {#toBool--}

Returns the property value as bool.

```javascript
toBool() : boolean;
```


**Remarks**

<p>Throws an exception if the property type is not PropertyType.Boolean.</p>


