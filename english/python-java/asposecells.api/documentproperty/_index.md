---
title: "DocumentProperty Class"
linktitle: "DocumentProperty"
articleTitle: "DocumentProperty"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a custom or built-in document property."
type: docs
weight: 1830
url: /python-java/asposecells.api/documentproperty/
---

## DocumentProperty class

Represents a custom or built-in document property.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Name](#name) | String | Returns the name of the property. |
| [Value](#value) | Object | Gets or sets the value of the property. |
| [IsLinkedToContent](#islinkedtocontent) | boolean | Indicates whether this property is linked to content |
| [Source](#source) | String | The linked content source. |
| [Type](#type) | int | Gets the data type of the property. The value of the property is PropertyType integer constant. |
| [IsGeneratedName](#isgeneratedname) | boolean | Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the publ |

## Methods

| Name | Description |
| --- | --- |
| [toString](#tostring) | Returns the property value as a string.

Converts a number property using Object.ToString(). Converts a boolean property |
| [toInt](#toint) | Returns the property value as integer.

Throws an exception if the property type is not PropertyType.Number. |
| [toDouble](#todouble) | Returns the property value as double.

Throws an exception if the property type is not PropertyType.Float. |
| [toDateTime](#todatetime) | Returns the property value as DateTime in local timezone.

Throws an exception if the property type is not PropertyType. |
| [toBool](#tobool) | Returns the property value as bool.

Throws an exception if the property type is not PropertyType.Boolean. |

### DocumentProperty.Name property {#name}

Returns the name of the property.

**Type:** String

### DocumentProperty.Value property {#value}

Gets or sets the value of the property.

**Type:** Object

### DocumentProperty.IsLinkedToContent property {#islinkedtocontent}

Indicates whether this property is linked to content

**Type:** boolean

### DocumentProperty.Source property {#source}

The linked content source.

**Type:** String

### DocumentProperty.Type property {#type}

Gets the data type of the property. The value of the property is PropertyType integer constant.

**Type:** int

### DocumentProperty.IsGeneratedName property {#isgeneratedname}

Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API.

**Type:** boolean

### toString() {#tostring}

Returns the property value as a string.

Converts a number property using Object.ToString(). Converts a boolean property into "Y" or "N". Converts a date property into a short date string.

### toInt() {#toint}

Returns the property value as integer.

Throws an exception if the property type is not PropertyType.Number.

### toDouble() {#todouble}

Returns the property value as double.

Throws an exception if the property type is not PropertyType.Float.

### toDateTime() {#todatetime}

Returns the property value as DateTime in local timezone.

Throws an exception if the property type is not PropertyType.Date.

### toBool() {#tobool}

Returns the property value as bool.

Throws an exception if the property type is not PropertyType.Boolean.
