---
title: "ListBoxActiveXControl"
linktitle: "ListBoxActiveXControl"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a ListBox ActiveX control."
type: docs
weight: 2090
url: /nodejs/aspose.cells/listboxactivexcontrol/
---

## ListBoxActiveXControl class

Represents a ListBox ActiveX control.

## Methods

| Name | Description |
| --- | --- |
| [getBackOleColor()](#getbackolecolor) | Gets and sets the ole color of the background. |
| [getBorderOleColor()](#getborderolecolor) | Gets and sets the ole color of the background. |
| [getBorderStyle()](#getborderstyle) | Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant. |
| [getBoundColumn()](#getboundcolumn) | Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMulti |
| [getColumnCount()](#getcolumncount) | Represents the number of columns to display in a ComboBox or ListBox. |
| [getColumnWidths()](#getcolumnwidths) | Gets and sets the width of the column. |
| [getData()](#getdata) | Gets and sets the binary data of the control. |
| [getFont()](#getfont) | Represents the font of the control. |
| [getForeOleColor()](#getforeolecolor) | Gets and sets the ole color of the foreground. Not applies to Image control. |
| [getHeight()](#getheight) | Gets and sets the height of the control in unit of points. |
| [getIMEMode()](#getimemode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of th |
| [getIntegralHeight()](#getintegralheight) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [getLinkedCell()](#getlinkedcell) | Gets and sets the linked cell. |
| [getListFillRange()](#getlistfillrange) | Gets and sets the list fill range. |
| [getListStyle()](#getliststyle) | Gets and sets the visual appearance. The value of the property is ControlListStyle integer constant. |
| [getListWidth()](#getlistwidth) | Gets and set the width in unit of points. |
| [getMatchEntry()](#getmatchentry) | Indicates how a ListBox or ComboBox searches its list as the user types. The value of the property is ControlMatchEntryT |
| [getMouseIcon()](#getmouseicon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getmousepointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMouse |
| [getScrollBars()](#getscrollbars) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. The value of |
| [getSelectionType()](#getselectiontype) | Indicates whether the control permits multiple selections. The value of the property is SelectionType integer constant. |
| [getShadow()](#getshadow) | Indicates whether to show a shadow. |
| [getShowColumnHeads()](#getshowcolumnheads) | Indicates whether column headings are displayed. |
| [getSpecialEffect()](#getspecialeffect) | Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant. |
| [getTextAlign()](#gettextalign) | Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant. |
| [getTextColumn()](#gettextcolumn) | Represents the column in a ComboBox or ListBox to display to the user. |
| [getType()](#gettype) | Gets the type of the ActiveX control. The value of the property is ControlType integer constant. |
| [getValue()](#getvalue) | Gets and sets the value of the control. Only effects when SelectionType is SelectionType.Single; |
| [getWidth()](#getwidth) | Gets and sets the width of the control in unit of points. |
| [getWorkbook()](#getworkbook) | Gets the Workbook object. |
| [isAutoSize()](#isautosize) | Indicates whether the control will automatically resize to display its entire contents. |
| [isEnabled()](#isenabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#islocked) | Indicates whether data in the control is locked for editing. |
| [isTransparent()](#istransparent) | Indicates whether the control is transparent. |
| [isVisible()](#isvisible) | Indicates whether this control is visible. |
| [setAutoSize()](#setautosize) | Indicates whether the control will automatically resize to display its entire contents. |
| [setBackOleColor()](#setbackolecolor) | Gets and sets the ole color of the background. |
| [setBorderOleColor()](#setborderolecolor) | Gets and sets the ole color of the background. |
| [setBorderStyle()](#setborderstyle) | Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant. |
| [setBoundColumn()](#setboundcolumn) | Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMulti |
| [setColumnCount()](#setcolumncount) | Represents the number of columns to display in a ComboBox or ListBox. |
| [setColumnWidths()](#setcolumnwidths) | Gets and sets the width of the column. |
| [setEnabled()](#setenabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [setForeOleColor()](#setforeolecolor) | Gets and sets the ole color of the foreground. Not applies to Image control. |
| [setHeight()](#setheight) | Gets and sets the height of the control in unit of points. |
| [setIMEMode()](#setimemode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of th |
| [setIntegralHeight()](#setintegralheight) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [setLinkedCell()](#setlinkedcell) | Gets and sets the linked cell. |
| [setListFillRange()](#setlistfillrange) | Gets and sets the list fill range. |
| [setListStyle()](#setliststyle) | Gets and sets the visual appearance. The value of the property is ControlListStyle integer constant. |
| [setListWidth()](#setlistwidth) | Gets and set the width in unit of points. |
| [setLocked()](#setlocked) | Indicates whether data in the control is locked for editing. |
| [setMatchEntry()](#setmatchentry) | Indicates how a ListBox or ComboBox searches its list as the user types. The value of the property is ControlMatchEntryT |
| [setMouseIcon()](#setmouseicon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [setMousePointer()](#setmousepointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMouse |
| [setScrollBars()](#setscrollbars) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. The value of |
| [setSelectionType()](#setselectiontype) | Indicates whether the control permits multiple selections. The value of the property is SelectionType integer constant. |
| [setShadow()](#setshadow) | Indicates whether to show a shadow. |
| [setShowColumnHeads()](#setshowcolumnheads) | Indicates whether column headings are displayed. |
| [setSpecialEffect()](#setspecialeffect) | Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant. |
| [setTextAlign()](#settextalign) | Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant. |
| [setTextColumn()](#settextcolumn) | Represents the column in a ComboBox or ListBox to display to the user. |
| [setTransparent()](#settransparent) | Indicates whether the control is transparent. |
| [setValue()](#setvalue) | Gets and sets the value of the control. Only effects when SelectionType is SelectionType.Single; |
| [setVisible()](#setvisible) | Indicates whether this control is visible. |
| [setWidth()](#setwidth) | Gets and sets the width of the control in unit of points. |

### getBackOleColor() {#getbackolecolor}

Gets and sets the ole color of the background.

### getBorderOleColor() {#getborderolecolor}

Gets and sets the ole color of the background.

### getBorderStyle() {#getborderstyle}

Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant.

### getBoundColumn() {#getboundcolumn}

Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle).

### getColumnCount() {#getcolumncount}

Represents the number of columns to display in a ComboBox or ListBox.

### getColumnWidths() {#getcolumnwidths}

Gets and sets the width of the column.

### getData() {#getdata}

Gets and sets the binary data of the control.

### getFont() {#getfont}

Represents the font of the control.

### getForeOleColor() {#getforeolecolor}

Gets and sets the ole color of the foreground. Not applies to Image control.

### getHeight() {#getheight}

Gets and sets the height of the control in unit of points.

### getIMEMode() {#getimemode}

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of the property is InputMethodEditorMode integer constant.

### getIntegralHeight() {#getintegralheight}

Indicates whether the control will only show complete lines of text without showing any partial lines.

### getLinkedCell() {#getlinkedcell}

Gets and sets the linked cell.

### getListFillRange() {#getlistfillrange}

Gets and sets the list fill range.

### getListStyle() {#getliststyle}

Gets and sets the visual appearance. The value of the property is ControlListStyle integer constant.

### getListWidth() {#getlistwidth}

Gets and set the width in unit of points.

### getMatchEntry() {#getmatchentry}

Indicates how a ListBox or ComboBox searches its list as the user types. The value of the property is ControlMatchEntryType integer constant.

### getMouseIcon() {#getmouseicon}

Gets and sets a custom icon to display as the mouse pointer for the control.

### getMousePointer() {#getmousepointer}

Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMousePointerType integer constant.

### getScrollBars() {#getscrollbars}

Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. The value of the property is ControlScrollBarType integer constant.

### getSelectionType() {#getselectiontype}

Indicates whether the control permits multiple selections. The value of the property is SelectionType integer constant.

### getShadow() {#getshadow}

Indicates whether to show a shadow.

### getShowColumnHeads() {#getshowcolumnheads}

Indicates whether column headings are displayed.

### getSpecialEffect() {#getspecialeffect}

Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant.

### getTextAlign() {#gettextalign}

Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant.

### getTextColumn() {#gettextcolumn}

Represents the column in a ComboBox or ListBox to display to the user.

### getType() {#gettype}

Gets the type of the ActiveX control. The value of the property is ControlType integer constant.

### getValue() {#getvalue}

Gets and sets the value of the control. Only effects when SelectionType is SelectionType.Single;

### getWidth() {#getwidth}

Gets and sets the width of the control in unit of points.

### getWorkbook() {#getworkbook}

Gets the Workbook object.

### isAutoSize() {#isautosize}

Indicates whether the control will automatically resize to display its entire contents.

### isEnabled() {#isenabled}

Indicates whether the control can receive the focus and respond to user-generated events.

### isLocked() {#islocked}

Indicates whether data in the control is locked for editing.

### isTransparent() {#istransparent}

Indicates whether the control is transparent.

### isVisible() {#isvisible}

Indicates whether this control is visible.

### setAutoSize() {#setautosize}

Indicates whether the control will automatically resize to display its entire contents.

### setBackOleColor() {#setbackolecolor}

Gets and sets the ole color of the background.

### setBorderOleColor() {#setborderolecolor}

Gets and sets the ole color of the background.

### setBorderStyle() {#setborderstyle}

Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant.

### setBoundColumn() {#setboundcolumn}

Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMultiSelectSingle).

### setColumnCount() {#setcolumncount}

Represents the number of columns to display in a ComboBox or ListBox.

### setColumnWidths() {#setcolumnwidths}

Gets and sets the width of the column.

### setEnabled() {#setenabled}

Indicates whether the control can receive the focus and respond to user-generated events.

### setForeOleColor() {#setforeolecolor}

Gets and sets the ole color of the foreground. Not applies to Image control.

### setHeight() {#setheight}

Gets and sets the height of the control in unit of points.

### setIMEMode() {#setimemode}

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of the property is InputMethodEditorMode integer constant.

### setIntegralHeight() {#setintegralheight}

Indicates whether the control will only show complete lines of text without showing any partial lines.

### setLinkedCell() {#setlinkedcell}

Gets and sets the linked cell.

### setListFillRange() {#setlistfillrange}

Gets and sets the list fill range.

### setListStyle() {#setliststyle}

Gets and sets the visual appearance. The value of the property is ControlListStyle integer constant.

### setListWidth() {#setlistwidth}

Gets and set the width in unit of points.

### setLocked() {#setlocked}

Indicates whether data in the control is locked for editing.

### setMatchEntry() {#setmatchentry}

Indicates how a ListBox or ComboBox searches its list as the user types. The value of the property is ControlMatchEntryType integer constant.

### setMouseIcon() {#setmouseicon}

Gets and sets a custom icon to display as the mouse pointer for the control.

### setMousePointer() {#setmousepointer}

Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMousePointerType integer constant.

### setScrollBars() {#setscrollbars}

Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. The value of the property is ControlScrollBarType integer constant.

### setSelectionType() {#setselectiontype}

Indicates whether the control permits multiple selections. The value of the property is SelectionType integer constant.

### setShadow() {#setshadow}

Indicates whether to show a shadow.

### setShowColumnHeads() {#setshowcolumnheads}

Indicates whether column headings are displayed.

### setSpecialEffect() {#setspecialeffect}

Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant.

### setTextAlign() {#settextalign}

Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant.

### setTextColumn() {#settextcolumn}

Represents the column in a ComboBox or ListBox to display to the user.

### setTransparent() {#settransparent}

Indicates whether the control is transparent.

### setValue() {#setvalue}

Gets and sets the value of the control. Only effects when SelectionType is SelectionType.Single;

### setVisible() {#setvisible}

Indicates whether this control is visible.

### setWidth() {#setwidth}

Gets and sets the width of the control in unit of points.
