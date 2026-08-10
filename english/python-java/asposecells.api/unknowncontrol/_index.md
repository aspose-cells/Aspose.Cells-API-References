---
title: "UnknownControl Class"
linktitle: "UnknownControl"
articleTitle: "UnknownControl"
second_title: "Aspose.Cells for Python via Java"
description: "Unknow control."
type: docs
weight: 7210
url: /python-java/asposecells.api/unknowncontrol/
---

## UnknownControl class

Unknow control.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Data](#data) | byte[] | Gets and sets the binary data of the control. |
| [Type](#type) | int | Gets the type of the ActiveX control. The value of the property is ControlType integer constant. |
| [IsEnabled](#isenabled) | boolean | Indicates whether the control can receive the focus and respond to user-generated events. |
| [IsLocked](#islocked) | boolean | Indicates whether data in the control is locked for editing. |
| [IsTransparent](#istransparent) | boolean | Indicates whether the control is transparent. |
| [IsAutoSize](#isautosize) | boolean | Indicates whether the control will automatically resize to display its entire contents. |
| [IMEMode](#imemode) | int | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of th |
| [Font](#font) | Font | Represents the font of the control. |
| [TextAlign](#textalign) | int | Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant. |
| [Workbook](#workbook) | Workbook | Gets the Workbook object. |
| [Width](#width) | float | Gets and sets the width of the control in unit of points. |
| [Height](#height) | float | Gets and sets the height of the control in unit of points. |
| [MouseIcon](#mouseicon) | byte[] | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [MousePointer](#mousepointer) | int | Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMouse |
| [ForeOleColor](#foreolecolor) | int | Gets and sets the ole color of the foreground. Not applies to Image control. |
| [BackOleColor](#backolecolor) | int | Gets and sets the ole color of the background. |
| [IsVisible](#isvisible) | boolean | Indicates whether this control is visible. |
| [Shadow](#shadow) | boolean | Indicates whether to show a shadow. |
| [LinkedCell](#linkedcell) | String | Gets and sets the linked cell. |
| [ListFillRange](#listfillrange) | String | Gets and sets the list fill range. |

## Methods

| Name | Description |
| --- | --- |
| [getRelationshipData](#getrelationshipdata) | Gets the related data. |

### UnknownControl.Data property {#data}

Gets and sets the binary data of the control.

**Type:** byte[]

### UnknownControl.Type property {#type}

Gets the type of the ActiveX control. The value of the property is ControlType integer constant.

**Type:** int

### UnknownControl.IsEnabled property {#isenabled}

Indicates whether the control can receive the focus and respond to user-generated events.

**Type:** boolean

### UnknownControl.IsLocked property {#islocked}

Indicates whether data in the control is locked for editing.

**Type:** boolean

### UnknownControl.IsTransparent property {#istransparent}

Indicates whether the control is transparent.

**Type:** boolean

### UnknownControl.IsAutoSize property {#isautosize}

Indicates whether the control will automatically resize to display its entire contents.

**Type:** boolean

### UnknownControl.IMEMode property {#imemode}

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of the property is InputMethodEditorMode integer constant.

**Type:** int

### UnknownControl.Font property {#font}

Represents the font of the control.

**Type:** Font

### UnknownControl.TextAlign property {#textalign}

Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant.

**Type:** int

### UnknownControl.Workbook property {#workbook}

Gets the Workbook object.

**Type:** Workbook

### UnknownControl.Width property {#width}

Gets and sets the width of the control in unit of points.

**Type:** float

### UnknownControl.Height property {#height}

Gets and sets the height of the control in unit of points.

**Type:** float

### UnknownControl.MouseIcon property {#mouseicon}

Gets and sets a custom icon to display as the mouse pointer for the control.

**Type:** byte[]

### UnknownControl.MousePointer property {#mousepointer}

Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMousePointerType integer constant.

**Type:** int

### UnknownControl.ForeOleColor property {#foreolecolor}

Gets and sets the ole color of the foreground. Not applies to Image control.

**Type:** int

### UnknownControl.BackOleColor property {#backolecolor}

Gets and sets the ole color of the background.

**Type:** int

### UnknownControl.IsVisible property {#isvisible}

Indicates whether this control is visible.

**Type:** boolean

### UnknownControl.Shadow property {#shadow}

Indicates whether to show a shadow.

**Type:** boolean

### UnknownControl.LinkedCell property {#linkedcell}

Gets and sets the linked cell.

**Type:** String

### UnknownControl.ListFillRange property {#listfillrange}

Gets and sets the list fill range.

**Type:** String

### getRelationshipData(relId) {#getrelationshipdata}

Gets the related data.

| Parameter | Type | Description |
| --- | --- | --- |
| relId | String | The relationship id. |

**Returns:** Returns the related data.
