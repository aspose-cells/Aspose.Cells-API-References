---
title: "DocumentProperty"
linktitle: "DocumentProperty"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a custom or built-in document property."
type: docs
weight: 1210
url: /nodejs/aspose.cells/documentproperty/
---

## DocumentProperty class

Represents a custom or built-in document property.

## Methods

| Name | Description |
| --- | --- |
| [getName()](#getname) | Returns the name of the property. |
| [getSource()](#getsource) | The linked content source. |
| [getType()](#gettype) | Gets the data type of the property. The value of the property is PropertyType integer constant. |
| [getValue()](#getvalue) | Gets or sets the value of the property. |
| [isGeneratedName()](#isgeneratedname) | Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the publ |
| [isLinkedToContent()](#islinkedtocontent) | Indicates whether this property is linked to content |
| [setValue()](#setvalue) | Gets or sets the value of the property. |
| [toBool()](#tobool) | Returns the property value as bool. Throws an exception if the property type is not PropertyType.Boolean. |
| [toDateTime()](#todatetime) | Returns the property value as DateTime in local timezone. Throws an exception if the property type is not PropertyType.D |
| [toDouble()](#todouble) | Returns the property value as double. Throws an exception if the property type is not PropertyType.Float. |
| [toInt()](#toint) | Returns the property value as integer. Throws an exception if the property type is not PropertyType.Number. |
| [toString()](#tostring) | Returns the property value as a string. Converts a number property using Object.ToString(). Converts a boolean property  |

### getName() {#getname}

Returns the name of the property.

### getSource() {#getsource}

The linked content source.

### getType() {#gettype}

Gets the data type of the property. The value of the property is PropertyType integer constant.

### getValue() {#getvalue}

Gets or sets the value of the property.

### isGeneratedName() {#isgeneratedname}

Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API.

### isLinkedToContent() {#islinkedtocontent}

Indicates whether this property is linked to content

### setValue() {#setvalue}

Gets or sets the value of the property.

### toBool() {#tobool}

Returns the property value as bool. Throws an exception if the property type is not PropertyType.Boolean.

### toDateTime() {#todatetime}

Returns the property value as DateTime in local timezone. Throws an exception if the property type is not PropertyType.Date.

### toDouble() {#todouble}

Returns the property value as double. Throws an exception if the property type is not PropertyType.Float.

### toInt() {#toint}

Returns the property value as integer. Throws an exception if the property type is not PropertyType.Number.

### toString() {#tostring}

Returns the property value as a string. Converts a number property using Object.ToString(). Converts a boolean property into "Y" or "N". Converts a date property into a short date string.
