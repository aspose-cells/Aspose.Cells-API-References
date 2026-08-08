---
title: "ComboBoxActiveXControl"
linktitle: "ComboBoxActiveXControl"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a ComboBox ActiveX control."
type: docs
weight: 710
url: /nodejs/aspose.cells/comboboxactivexcontrol/
---

## ComboBoxActiveXControl class

Represents a ComboBox ActiveX control.

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
| [getDropButtonStyle()](#getdropbuttonstyle) | Specifies the symbol displayed on the drop button The value of the property is DropButtonStyle integer constant. |
| [getEnterFieldBehavior()](#getenterfieldbehavior) | Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last ti |
| [getFont()](#getfont) | Represents the font of the control. |
| [getForeOleColor()](#getforeolecolor) | Gets and sets the ole color of the foreground. Not applies to Image control. |
| [getHeight()](#getheight) | Gets and sets the height of the control in unit of points. |
| [getHideSelection()](#gethideselection) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [getIMEMode()](#getimemode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of th |
| [getLinkedCell()](#getlinkedcell) | Gets and sets the linked cell. |
| [getListFillRange()](#getlistfillrange) | Gets and sets the list fill range. |
| [getListRows()](#getlistrows) | Represents the maximum number of rows to display in the list. |
| [getListStyle()](#getliststyle) | Gets and sets the visual appearance. The value of the property is ControlListStyle integer constant. |
| [getListWidth()](#getlistwidth) | Gets and set the width in unit of points. |
| [getMatchEntry()](#getmatchentry) | Indicates how a ListBox or ComboBox searches its list as the user types. The value of the property is ControlMatchEntryT |
| [getMaxLength()](#getmaxlength) | Gets and sets the maximum number of characters |
| [getMouseIcon()](#getmouseicon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getmousepointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMouse |
| [getSelectionMargin()](#getselectionmargin) | Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
| [getShadow()](#getshadow) | Indicates whether to show a shadow. |
| [getShowColumnHeads()](#getshowcolumnheads) | Indicates whether column headings are displayed. |
| [getShowDropButtonTypeWhen()](#getshowdropbuttontypewhen) | Specifies the symbol displayed on the drop button The value of the property is ShowDropButtonType integer constant. |
| [getSpecialEffect()](#getspecialeffect) | Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant. |
| [getTextAlign()](#gettextalign) | Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant. |
| [getTextColumn()](#gettextcolumn) | Represents the column in a ComboBox or ListBox to display to the user. |
| [getType()](#gettype) | Gets the type of the ActiveX control. The value of the property is ControlType integer constant. |
| [getValue()](#getvalue) | Gets and sets the value of the control. |
| [getWidth()](#getwidth) | Gets and sets the width of the control in unit of points. |
| [getWorkbook()](#getworkbook) | Gets the Workbook object. |
| [isAutoSize()](#isautosize) | Indicates whether the control will automatically resize to display its entire contents. |
| [isAutoWordSelected()](#isautowordselected) | Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false spe |
| [isDragBehaviorEnabled()](#isdragbehaviorenabled) | Indicates whether dragging and dropping is enabled for the control. |
| [isEditable()](#iseditable) | Indicates whether the user can type into the control. |
| [isEnabled()](#isenabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#islocked) | Indicates whether data in the control is locked for editing. |
| [isTransparent()](#istransparent) | Indicates whether the control is transparent. |
| [isVisible()](#isvisible) | Indicates whether this control is visible. |
| [setAutoSize()](#setautosize) | Indicates whether the control will automatically resize to display its entire contents. |
| [setAutoWordSelected()](#setautowordselected) | Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false spe |
| [setBackOleColor()](#setbackolecolor) | Gets and sets the ole color of the background. |
| [setBorderOleColor()](#setborderolecolor) | Gets and sets the ole color of the background. |
| [setBorderStyle()](#setborderstyle) | Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant. |
| [setBoundColumn()](#setboundcolumn) | Represents how the Value property is determined for a ComboBox or ListBox when the MultiSelect properties value (fmMulti |
| [setColumnCount()](#setcolumncount) | Represents the number of columns to display in a ComboBox or ListBox. |
| [setColumnWidths()](#setcolumnwidths) | Gets and sets the width of the column. |
| [setDragBehaviorEnabled()](#setdragbehaviorenabled) | Indicates whether dragging and dropping is enabled for the control. |
| [setDropButtonStyle()](#setdropbuttonstyle) | Specifies the symbol displayed on the drop button The value of the property is DropButtonStyle integer constant. |
| [setEditable()](#seteditable) | Indicates whether the user can type into the control. |
| [setEnabled()](#setenabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [setEnterFieldBehavior()](#setenterfieldbehavior) | Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last ti |
| [setForeOleColor()](#setforeolecolor) | Gets and sets the ole color of the foreground. Not applies to Image control. |
| [setHeight()](#setheight) | Gets and sets the height of the control in unit of points. |
| [setHideSelection()](#sethideselection) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [setIMEMode()](#setimemode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of th |
| [setLinkedCell()](#setlinkedcell) | Gets and sets the linked cell. |
| [setListFillRange()](#setlistfillrange) | Gets and sets the list fill range. |
| [setListRows()](#setlistrows) | Represents the maximum number of rows to display in the list. |
| [setListStyle()](#setliststyle) | Gets and sets the visual appearance. The value of the property is ControlListStyle integer constant. |
| [setListWidth()](#setlistwidth) | Gets and set the width in unit of points. |
| [setLocked()](#setlocked) | Indicates whether data in the control is locked for editing. |
| [setMatchEntry()](#setmatchentry) | Indicates how a ListBox or ComboBox searches its list as the user types. The value of the property is ControlMatchEntryT |
| [setMaxLength()](#setmaxlength) | Gets and sets the maximum number of characters |
| [setMouseIcon()](#setmouseicon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [setMousePointer()](#setmousepointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMouse |
| [setSelectionMargin()](#setselectionmargin) | Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
| [setShadow()](#setshadow) | Indicates whether to show a shadow. |
| [setShowColumnHeads()](#setshowcolumnheads) | Indicates whether column headings are displayed. |
| [setShowDropButtonTypeWhen()](#setshowdropbuttontypewhen) | Specifies the symbol displayed on the drop button The value of the property is ShowDropButtonType integer constant. |
| [setSpecialEffect()](#setspecialeffect) | Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant. |
| [setTextAlign()](#settextalign) | Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant. |
| [setTextColumn()](#settextcolumn) | Represents the column in a ComboBox or ListBox to display to the user. |
| [setTransparent()](#settransparent) | Indicates whether the control is transparent. |
| [setValue()](#setvalue) | Gets and sets the value of the control. |
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

### getDropButtonStyle() {#getdropbuttonstyle}

Specifies the symbol displayed on the drop button The value of the property is DropButtonStyle integer constant.

### getEnterFieldBehavior() {#getenterfieldbehavior}

Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.

### getFont() {#getfont}

Represents the font of the control.

### getForeOleColor() {#getforeolecolor}

Gets and sets the ole color of the foreground. Not applies to Image control.

### getHeight() {#getheight}

Gets and sets the height of the control in unit of points.

### getHideSelection() {#gethideselection}

Indicates whether selected text in the control appears highlighted when the control does not have focus.

### getIMEMode() {#getimemode}

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of the property is InputMethodEditorMode integer constant.

### getLinkedCell() {#getlinkedcell}

Gets and sets the linked cell.

### getListFillRange() {#getlistfillrange}

Gets and sets the list fill range.

### getListRows() {#getlistrows}

Represents the maximum number of rows to display in the list.

### getListStyle() {#getliststyle}

Gets and sets the visual appearance. The value of the property is ControlListStyle integer constant.

### getListWidth() {#getlistwidth}

Gets and set the width in unit of points.

### getMatchEntry() {#getmatchentry}

Indicates how a ListBox or ComboBox searches its list as the user types. The value of the property is ControlMatchEntryType integer constant.

### getMaxLength() {#getmaxlength}

Gets and sets the maximum number of characters

### getMouseIcon() {#getmouseicon}

Gets and sets a custom icon to display as the mouse pointer for the control.

### getMousePointer() {#getmousepointer}

Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMousePointerType integer constant.

### getSelectionMargin() {#getselectionmargin}

Indicates whether the user can select a line of text by clicking in the region to the left of the text.

### getShadow() {#getshadow}

Indicates whether to show a shadow.

### getShowColumnHeads() {#getshowcolumnheads}

Indicates whether column headings are displayed.

### getShowDropButtonTypeWhen() {#getshowdropbuttontypewhen}

Specifies the symbol displayed on the drop button The value of the property is ShowDropButtonType integer constant.

### getSpecialEffect() {#getspecialeffect}

Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant.

### getTextAlign() {#gettextalign}

Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant.

### getTextColumn() {#gettextcolumn}

Represents the column in a ComboBox or ListBox to display to the user.

### getType() {#gettype}

Gets the type of the ActiveX control. The value of the property is ControlType integer constant.

### getValue() {#getvalue}

Gets and sets the value of the control.

### getWidth() {#getwidth}

Gets and sets the width of the control in unit of points.

### getWorkbook() {#getworkbook}

Gets the Workbook object.

### isAutoSize() {#isautosize}

Indicates whether the control will automatically resize to display its entire contents.

### isAutoWordSelected() {#isautowordselected}

Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.

### isDragBehaviorEnabled() {#isdragbehaviorenabled}

Indicates whether dragging and dropping is enabled for the control.

### isEditable() {#iseditable}

Indicates whether the user can type into the control.

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

### setAutoWordSelected() {#setautowordselected}

Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.

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

### setDragBehaviorEnabled() {#setdragbehaviorenabled}

Indicates whether dragging and dropping is enabled for the control.

### setDropButtonStyle() {#setdropbuttonstyle}

Specifies the symbol displayed on the drop button The value of the property is DropButtonStyle integer constant.

### setEditable() {#seteditable}

Indicates whether the user can type into the control.

### setEnabled() {#setenabled}

Indicates whether the control can receive the focus and respond to user-generated events.

### setEnterFieldBehavior() {#setenterfieldbehavior}

Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.

### setForeOleColor() {#setforeolecolor}

Gets and sets the ole color of the foreground. Not applies to Image control.

### setHeight() {#setheight}

Gets and sets the height of the control in unit of points.

### setHideSelection() {#sethideselection}

Indicates whether selected text in the control appears highlighted when the control does not have focus.

### setIMEMode() {#setimemode}

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of the property is InputMethodEditorMode integer constant.

### setLinkedCell() {#setlinkedcell}

Gets and sets the linked cell.

### setListFillRange() {#setlistfillrange}

Gets and sets the list fill range.

### setListRows() {#setlistrows}

Represents the maximum number of rows to display in the list.

### setListStyle() {#setliststyle}

Gets and sets the visual appearance. The value of the property is ControlListStyle integer constant.

### setListWidth() {#setlistwidth}

Gets and set the width in unit of points.

### setLocked() {#setlocked}

Indicates whether data in the control is locked for editing.

### setMatchEntry() {#setmatchentry}

Indicates how a ListBox or ComboBox searches its list as the user types. The value of the property is ControlMatchEntryType integer constant.

### setMaxLength() {#setmaxlength}

Gets and sets the maximum number of characters

### setMouseIcon() {#setmouseicon}

Gets and sets a custom icon to display as the mouse pointer for the control.

### setMousePointer() {#setmousepointer}

Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMousePointerType integer constant.

### setSelectionMargin() {#setselectionmargin}

Indicates whether the user can select a line of text by clicking in the region to the left of the text.

### setShadow() {#setshadow}

Indicates whether to show a shadow.

### setShowColumnHeads() {#setshowcolumnheads}

Indicates whether column headings are displayed.

### setShowDropButtonTypeWhen() {#setshowdropbuttontypewhen}

Specifies the symbol displayed on the drop button The value of the property is ShowDropButtonType integer constant.

### setSpecialEffect() {#setspecialeffect}

Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant.

### setTextAlign() {#settextalign}

Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant.

### setTextColumn() {#settextcolumn}

Represents the column in a ComboBox or ListBox to display to the user.

### setTransparent() {#settransparent}

Indicates whether the control is transparent.

### setValue() {#setvalue}

Gets and sets the value of the control.

### setVisible() {#setvisible}

Indicates whether this control is visible.

### setWidth() {#setwidth}

Gets and sets the width of the control in unit of points.
