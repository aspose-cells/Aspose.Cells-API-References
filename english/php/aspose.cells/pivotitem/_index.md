---
title: "PivotItem Class"
linktitle: "PivotItem"
articleTitle: "PivotItem"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a item in a PivotField report."
type: docs
weight: 4710
url: /php/aspose.cells/pivotitem/
---

## PivotItem class

Represents a item in a PivotField report.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsHidden](#ishidden) | boolean | Gets and Sets whether the pivot item is hidden. |
| [Position](#position) | Number | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [PositionInSameParentNode](#positioninsameparentnode) | Number | Specifying the position index in the PivotItems under the same parent node. |
| [IsHideDetail](#ishidedetail) | boolean | Gets and Sets whether the pivot item hides detail. |
| [IsDetailHidden](#isdetailhidden) | boolean |  |
| [IsCalculatedItem](#iscalculateditem) | boolean |  |
| [IsFormula](#isformula) | boolean | Indicates whether this pivot item is a calculated formula item. |
| [IsMissing](#ismissing) | boolean | Indicates whether the item is removed from the data source. True means this value has benn removed from the data source. |
| [Value](#value) | Object | Gets the value of the pivot item |
| [Name](#name) | String | Gets the name of the pivot item. |
| [Index](#index) | Number | Gets the index of the pivot item in cache field. |

## Methods

| Name | Description |
| --- | --- |
| [hide](#hide) | Sets whether the pivot item is hidden.

NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Pivot.PivotF |
| [move](#move) | Moves the item up or down |
| [getFormula](#getformula) |  |
| [getStringValue](#getstringvalue) | Gets the string value of the pivot item If the value is null, it will return "" |
| [getDoubleValue](#getdoublevalue) | Gets the double value of the pivot item If the value is null or not number ,it will return 0 |
| [getDateTimeValue](#getdatetimevalue) | Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue |

### PivotItem.IsHidden property {#ishidden}

Gets and Sets whether the pivot item is hidden.

**Type:** boolean

### PivotItem.Position property {#position}

Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

**Type:** Number

### PivotItem.PositionInSameParentNode property {#positioninsameparentnode}

Specifying the position index in the PivotItems under the same parent node.

**Type:** Number

### PivotItem.IsHideDetail property {#ishidedetail}

Gets and Sets whether the pivot item hides detail.

**Type:** boolean

### PivotItem.IsDetailHidden property {#isdetailhidden}

**Type:** boolean

### PivotItem.IsCalculatedItem property {#iscalculateditem}

**Type:** boolean

### PivotItem.IsFormula property {#isformula}

Indicates whether this pivot item is a calculated formula item.

**Type:** boolean

### PivotItem.IsMissing property {#ismissing}

Indicates whether the item is removed from the data source. True means this value has benn removed from the data source.

**Type:** boolean

### PivotItem.Value property {#value}

Gets the value of the pivot item

**Type:** Object

### PivotItem.Name property {#name}

Gets the name of the pivot item.

**Type:** String

### PivotItem.Index property {#index}

Gets the index of the pivot item in cache field.

**Type:** Number

### hide(value) {#hide}

Sets whether the pivot item is hidden.

NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Pivot.PivotField.HideItem method. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### move(count, isSameParent) {#move}

Moves the item up or down

| Parameter | Type | Description |
| --- | --- | --- |
| count | Number | The number of moving up or down. Move the item up if this is less than zero; Move the item down if this is greater than zero. |
| isSameParent | boolean | Specifying whether moving operation is in the same parent node or not |

### getFormula() {#getformula}

### getStringValue() {#getstringvalue}

Gets the string value of the pivot item If the value is null, it will return ""

### getDoubleValue() {#getdoublevalue}

Gets the double value of the pivot item If the value is null or not number ,it will return 0

### getDateTimeValue() {#getdatetimevalue}

Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue
