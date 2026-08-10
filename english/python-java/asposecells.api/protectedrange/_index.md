---
title: "ProtectedRange Class"
linktitle: "ProtectedRange"
articleTitle: "ProtectedRange"
second_title: "Aspose.Cells for Python via Java"
description: "A specified range to be allowed to edit when the sheet protection is ON."
type: docs
weight: 5170
url: /python-java/asposecells.api/protectedrange/
---

## ProtectedRange class

A specified range to be allowed to edit when the sheet protection is ON.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Name](#name) | String | Gets the Range title. This is used as a descriptor, not as a named range definition. |
| [CellArea](#cellarea) | CellArea | Gets the CellArea object represents the cell area to be protected. |
| [IsProtectedWithPassword](#isprotectedwithpassword) | boolean | Indicates whether the worksheets is protected with password. |
| [Password](#password) | String | Represents the password to protect the range. |
| [SecurityDescriptor](#securitydescriptor) | String | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |

## Methods

| Name | Description |
| --- | --- |
| [getAreas](#getareas) | Gets all referred areas. |
| [addArea](#addarea) | Adds a referred area to this |

### ProtectedRange.Name property {#name}

Gets the Range title. This is used as a descriptor, not as a named range definition.

**Type:** String

### ProtectedRange.CellArea property {#cellarea}

Gets the CellArea object represents the cell area to be protected.

**Type:** CellArea

### ProtectedRange.IsProtectedWithPassword property {#isprotectedwithpassword}

Indicates whether the worksheets is protected with password.

**Type:** boolean

### ProtectedRange.Password property {#password}

Represents the password to protect the range.

**Type:** String

### ProtectedRange.SecurityDescriptor property {#securitydescriptor}

The security descriptor defines user accounts who may edit this range without providing a password to access the range.

**Type:** String

### getAreas() {#getareas}

Gets all referred areas.

**Returns:** Returns all referred areas.

### addArea(startRow, startColumn, endRow, endColumn) {#addarea}

Adds a referred area to this

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row. |
| startColumn | int | The start column. |
| endRow | int | The end row. |
| endColumn | int | The end column. |
