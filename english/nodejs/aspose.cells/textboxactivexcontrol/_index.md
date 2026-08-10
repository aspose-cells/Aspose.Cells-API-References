---
title: "TextBoxActiveXControl"
linktitle: "TextBoxActiveXControl"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a text box ActiveX control."
type: docs
weight: 4080
url: /nodejs/aspose.cells/textboxactivexcontrol/
---

## TextBoxActiveXControl class

Represents a text box ActiveX control.

## Methods

| Name | Description |
| --- | --- |
| [getBackOleColor()](#getbackolecolor) | Gets and sets the ole color of the background. |
| [getBorderOleColor()](#getborderolecolor) | Gets and sets the ole color of the background. |
| [getBorderStyle()](#getborderstyle) | Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant. |
| [getData()](#getdata) | Gets and sets the binary data of the control. |
| [getDropButtonStyle()](#getdropbuttonstyle) | Specifies the symbol displayed on the drop button The value of the property is DropButtonStyle integer constant. |
| [getEnterFieldBehavior()](#getenterfieldbehavior) | Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last ti |
| [getEnterKeyBehavior()](#getenterkeybehavior) | Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that |
| [getFont()](#getfont) | Represents the font of the control. |
| [getForeOleColor()](#getforeolecolor) | Gets and sets the ole color of the foreground. Not applies to Image control. |
| [getHeight()](#getheight) | Gets and sets the height of the control in unit of points. |
| [getHideSelection()](#gethideselection) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [getIMEMode()](#getimemode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of th |
| [getIntegralHeight()](#getintegralheight) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [getLinkedCell()](#getlinkedcell) | Gets and sets the linked cell. |
| [getListFillRange()](#getlistfillrange) | Gets and sets the list fill range. |
| [getMaxLength()](#getmaxlength) | Gets and sets the maximum number of characters |
| [getMouseIcon()](#getmouseicon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [getMousePointer()](#getmousepointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMouse |
| [getPasswordChar()](#getpasswordchar) | Gets and sets a character to be displayed in place of the characters entered. |
| [getScrollBars()](#getscrollbars) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. The value of |
| [getShadow()](#getshadow) | Indicates whether to show a shadow. |
| [getShowDropButtonTypeWhen()](#getshowdropbuttontypewhen) | Specifies the symbol displayed on the drop button The value of the property is ShowDropButtonType integer constant. |
| [getSpecialEffect()](#getspecialeffect) | Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant. |
| [getTabKeyBehavior()](#gettabkeybehavior) | Indicates whether tab characters are allowed in the text of the control. |
| [getText()](#gettext) | Gets and set text of the control. |
| [getTextAlign()](#gettextalign) | Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant. |
| [getType()](#gettype) | Gets the type of the ActiveX control. The value of the property is ControlType integer constant. |
| [getWidth()](#getwidth) | Gets and sets the width of the control in unit of points. |
| [getWorkbook()](#getworkbook) | Gets the Workbook object. |
| [isAutoSize()](#isautosize) | Indicates whether the control will automatically resize to display its entire contents. |
| [isAutoTab()](#isautotab) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of chara |
| [isAutoWordSelected()](#isautowordselected) | Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false spe |
| [isDragBehaviorEnabled()](#isdragbehaviorenabled) | Indicates whether dragging and dropping is enabled for the control. |
| [isEditable()](#iseditable) | Indicates whether the user can type into the control. |
| [isEnabled()](#isenabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [isLocked()](#islocked) | Indicates whether data in the control is locked for editing. |
| [isMultiLine()](#ismultiline) | Indicates whether the control can display more than one line of text. |
| [isTransparent()](#istransparent) | Indicates whether the control is transparent. |
| [isVisible()](#isvisible) | Indicates whether this control is visible. |
| [isWordWrapped()](#iswordwrapped) | Indicates whether the contents of the control automatically wrap at the end of a line. |
| [setAutoSize()](#setautosize) | Indicates whether the control will automatically resize to display its entire contents. |
| [setAutoTab()](#setautotab) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of chara |
| [setAutoWordSelected()](#setautowordselected) | Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false spe |
| [setBackOleColor()](#setbackolecolor) | Gets and sets the ole color of the background. |
| [setBorderOleColor()](#setborderolecolor) | Gets and sets the ole color of the background. |
| [setBorderStyle()](#setborderstyle) | Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant. |
| [setDragBehaviorEnabled()](#setdragbehaviorenabled) | Indicates whether dragging and dropping is enabled for the control. |
| [setDropButtonStyle()](#setdropbuttonstyle) | Specifies the symbol displayed on the drop button The value of the property is DropButtonStyle integer constant. |
| [setEditable()](#seteditable) | Indicates whether the user can type into the control. |
| [setEnabled()](#setenabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [setEnterFieldBehavior()](#setenterfieldbehavior) | Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last ti |
| [setEnterKeyBehavior()](#setenterkeybehavior) | Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that |
| [setForeOleColor()](#setforeolecolor) | Gets and sets the ole color of the foreground. Not applies to Image control. |
| [setHeight()](#setheight) | Gets and sets the height of the control in unit of points. |
| [setHideSelection()](#sethideselection) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [setIMEMode()](#setimemode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of th |
| [setIntegralHeight()](#setintegralheight) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [setLinkedCell()](#setlinkedcell) | Gets and sets the linked cell. |
| [setListFillRange()](#setlistfillrange) | Gets and sets the list fill range. |
| [setLocked()](#setlocked) | Indicates whether data in the control is locked for editing. |
| [setMaxLength()](#setmaxlength) | Gets and sets the maximum number of characters |
| [setMouseIcon()](#setmouseicon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [setMousePointer()](#setmousepointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMouse |
| [setMultiLine()](#setmultiline) | Indicates whether the control can display more than one line of text. |
| [setPasswordChar()](#setpasswordchar) | Gets and sets a character to be displayed in place of the characters entered. |
| [setScrollBars()](#setscrollbars) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. The value of |
| [setShadow()](#setshadow) | Indicates whether to show a shadow. |
| [setShowDropButtonTypeWhen()](#setshowdropbuttontypewhen) | Specifies the symbol displayed on the drop button The value of the property is ShowDropButtonType integer constant. |
| [setSpecialEffect()](#setspecialeffect) | Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant. |
| [setTabKeyBehavior()](#settabkeybehavior) | Indicates whether tab characters are allowed in the text of the control. |
| [setText()](#settext) | Gets and set text of the control. |
| [setTextAlign()](#settextalign) | Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant. |
| [setTransparent()](#settransparent) | Indicates whether the control is transparent. |
| [setVisible()](#setvisible) | Indicates whether this control is visible. |
| [setWidth()](#setwidth) | Gets and sets the width of the control in unit of points. |
| [setWordWrapped()](#setwordwrapped) | Indicates whether the contents of the control automatically wrap at the end of a line. |

### getBackOleColor() {#getbackolecolor}

Gets and sets the ole color of the background.

### getBorderOleColor() {#getborderolecolor}

Gets and sets the ole color of the background.

### getBorderStyle() {#getborderstyle}

Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant.

### getData() {#getdata}

Gets and sets the binary data of the control.

### getDropButtonStyle() {#getdropbuttonstyle}

Specifies the symbol displayed on the drop button The value of the property is DropButtonStyle integer constant.

### getEnterFieldBehavior() {#getenterfieldbehavior}

Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.

### getEnterKeyBehavior() {#getenterkeybehavior}

Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that pressing ENTER will move the focus to the next object in the tab order.

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

### getIntegralHeight() {#getintegralheight}

Indicates whether the control will only show complete lines of text without showing any partial lines.

### getLinkedCell() {#getlinkedcell}

Gets and sets the linked cell.

### getListFillRange() {#getlistfillrange}

Gets and sets the list fill range.

### getMaxLength() {#getmaxlength}

Gets and sets the maximum number of characters

### getMouseIcon() {#getmouseicon}

Gets and sets a custom icon to display as the mouse pointer for the control.

### getMousePointer() {#getmousepointer}

Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMousePointerType integer constant.

### getPasswordChar() {#getpasswordchar}

Gets and sets a character to be displayed in place of the characters entered.

### getScrollBars() {#getscrollbars}

Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. The value of the property is ControlScrollBarType integer constant.

### getShadow() {#getshadow}

Indicates whether to show a shadow.

### getShowDropButtonTypeWhen() {#getshowdropbuttontypewhen}

Specifies the symbol displayed on the drop button The value of the property is ShowDropButtonType integer constant.

### getSpecialEffect() {#getspecialeffect}

Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant.

### getTabKeyBehavior() {#gettabkeybehavior}

Indicates whether tab characters are allowed in the text of the control.

### getText() {#gettext}

Gets and set text of the control.

### getTextAlign() {#gettextalign}

Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant.

### getType() {#gettype}

Gets the type of the ActiveX control. The value of the property is ControlType integer constant.

### getWidth() {#getwidth}

Gets and sets the width of the control in unit of points.

### getWorkbook() {#getworkbook}

Gets the Workbook object.

### isAutoSize() {#isautosize}

Indicates whether the control will automatically resize to display its entire contents.

### isAutoTab() {#isautotab}

Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters.

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

### isMultiLine() {#ismultiline}

Indicates whether the control can display more than one line of text.

### isTransparent() {#istransparent}

Indicates whether the control is transparent.

### isVisible() {#isvisible}

Indicates whether this control is visible.

### isWordWrapped() {#iswordwrapped}

Indicates whether the contents of the control automatically wrap at the end of a line.

### setAutoSize() {#setautosize}

Indicates whether the control will automatically resize to display its entire contents.

### setAutoTab() {#setautotab}

Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters.

### setAutoWordSelected() {#setautowordselected}

Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.

### setBackOleColor() {#setbackolecolor}

Gets and sets the ole color of the background.

### setBorderOleColor() {#setborderolecolor}

Gets and sets the ole color of the background.

### setBorderStyle() {#setborderstyle}

Gets and set the type of border used by the control. The value of the property is ControlBorderType integer constant.

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

### setEnterKeyBehavior() {#setenterkeybehavior}

Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that pressing ENTER will move the focus to the next object in the tab order.

### setForeOleColor() {#setforeolecolor}

Gets and sets the ole color of the foreground. Not applies to Image control.

### setHeight() {#setheight}

Gets and sets the height of the control in unit of points.

### setHideSelection() {#sethideselection}

Indicates whether selected text in the control appears highlighted when the control does not have focus.

### setIMEMode() {#setimemode}

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. The value of the property is InputMethodEditorMode integer constant.

### setIntegralHeight() {#setintegralheight}

Indicates whether the control will only show complete lines of text without showing any partial lines.

### setLinkedCell() {#setlinkedcell}

Gets and sets the linked cell.

### setListFillRange() {#setlistfillrange}

Gets and sets the list fill range.

### setLocked() {#setlocked}

Indicates whether data in the control is locked for editing.

### setMaxLength() {#setmaxlength}

Gets and sets the maximum number of characters

### setMouseIcon() {#setmouseicon}

Gets and sets a custom icon to display as the mouse pointer for the control.

### setMousePointer() {#setmousepointer}

Gets and sets the type of icon displayed as the mouse pointer for the control. The value of the property is ControlMousePointerType integer constant.

### setMultiLine() {#setmultiline}

Indicates whether the control can display more than one line of text.

### setPasswordChar() {#setpasswordchar}

Gets and sets a character to be displayed in place of the characters entered.

### setScrollBars() {#setscrollbars}

Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. The value of the property is ControlScrollBarType integer constant.

### setShadow() {#setshadow}

Indicates whether to show a shadow.

### setShowDropButtonTypeWhen() {#setshowdropbuttontypewhen}

Specifies the symbol displayed on the drop button The value of the property is ShowDropButtonType integer constant.

### setSpecialEffect() {#setspecialeffect}

Gets and sets the special effect of the control. The value of the property is ControlSpecialEffectType integer constant.

### setTabKeyBehavior() {#settabkeybehavior}

Indicates whether tab characters are allowed in the text of the control.

### setText() {#settext}

Gets and set text of the control.

### setTextAlign() {#settextalign}

Represents how to align the text used by the control. The value of the property is TextAlignmentType integer constant.

### setTransparent() {#settransparent}

Indicates whether the control is transparent.

### setVisible() {#setvisible}

Indicates whether this control is visible.

### setWidth() {#setwidth}

Gets and sets the width of the control in unit of points.

### setWordWrapped() {#setwordwrapped}

Indicates whether the contents of the control automatically wrap at the end of a line.
