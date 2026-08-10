---
title: "FindOptions Class"
linktitle: "FindOptions"
articleTitle: "FindOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents find options."
type: docs
weight: 2400
url: /python-java/asposecells.api/findoptions/
---

## FindOptions class

Represents find options.

## Constructors

| Name | Description |
| --- | --- |
| [FindOptions](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CaseSensitive](#casesensitive) | boolean | Indicates if the searched string is case sensitive. |
| [LookAtType](#lookattype) | int | Look at type. The value of the property is LookAtType integer constant. |
| [IsRangeSet](#israngeset) | boolean | Indicates whether the searched range is set. |
| [SearchNext](#searchnext) | boolean | Search order. True: search next. False: search previous. NOTE: This member is now obsolete. Instead, please use FindOpti |
| [SearchBackward](#searchbackward) | boolean | Whether search backward for cells. |
| [SeachOrderByRows](#seachorderbyrows) | boolean | Indicates whether search order by rows or columns. |
| [SearchOrderByRows](#searchorderbyrows) | boolean |  |
| [LookInType](#lookintype) | int | Look in type. The value of the property is LookInType integer constant. |
| [RegexKey](#regexkey) | boolean | Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the k |
| [ValueTypeSensitive](#valuetypesensitive) | boolean | Indicates whether searched cell value type should be same with the searched key. |
| [Style](#style) | Style | The format to search for. |
| [ConvertNumericData](#convertnumericdata) | boolean | Gets or sets a value that indicates whether converting the searched string value to numeric data. |

## Methods

| Name | Description |
| --- | --- |
| [getRange](#getrange) | Gets and sets the searched range. |
| [setRange](#setrange) | Sets the searched range. |

### FindOptions() {#constructor}

### FindOptions.CaseSensitive property {#casesensitive}

Indicates if the searched string is case sensitive.

**Type:** boolean

### FindOptions.LookAtType property {#lookattype}

Look at type. The value of the property is LookAtType integer constant.

**Type:** int

### FindOptions.IsRangeSet property {#israngeset}

Indicates whether the searched range is set.

**Type:** boolean

### FindOptions.SearchNext property {#searchnext}

Search order. True: search next. False: search previous. NOTE: This member is now obsolete. Instead, please use FindOptions.SearchBackward property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### FindOptions.SearchBackward property {#searchbackward}

Whether search backward for cells.

**Type:** boolean

### FindOptions.SeachOrderByRows property {#seachorderbyrows}

Indicates whether search order by rows or columns.

**Type:** boolean

### FindOptions.SearchOrderByRows property {#searchorderbyrows}

**Type:** boolean

### FindOptions.LookInType property {#lookintype}

Look in type. The value of the property is LookInType integer constant.

**Type:** int

### FindOptions.RegexKey property {#regexkey}

Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.

**Type:** boolean

### FindOptions.ValueTypeSensitive property {#valuetypesensitive}

Indicates whether searched cell value type should be same with the searched key.

**Type:** boolean

### FindOptions.Style property {#style}

The format to search for.

**Type:** Style

### FindOptions.ConvertNumericData property {#convertnumericdata}

Gets or sets a value that indicates whether converting the searched string value to numeric data.

**Type:** boolean

### getRange() {#getrange}

Gets and sets the searched range.

**Returns:** Returns the searched range.

### setRange(ca) {#setrange}

Sets the searched range.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the searched range. |
