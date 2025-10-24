##StyleModifyFlag
The style modified flags.
**Inheritance:**
java.lang.Object
```
public final class StyleModifyFlag
```
The style modified flags.
**Remarks**
Combinations of multiple properties are defined for user's convenience. When checking whether they are modified for one style, the returned value denotes whether one or more properties in the combination have been modified.
## Fields
| Field | Description |
| --- | --- |
| [ALIGNMENT_SETTINGS](#ALIGNMENT-SETTINGS) | Indicates whether one or more alignment-related properties([HORIZONTAL\_ALIGNMENT](../../com.aspose.cells/stylemodifyflag\#HORIZONTAL-ALIGNMENT), [VERTICAL\_ALIGNMENT](../../com.aspose.cells/stylemodifyflag\#VERTICAL-ALIGNMENT), [ROTATION](../../com.aspose.cells/stylemodifyflag\#ROTATION), [WRAP\_TEXT](../../com.aspose.cells/stylemodifyflag\#WRAP-TEXT), [WRAP\_TEXT](../../com.aspose.cells/stylemodifyflag\#WRAP-TEXT), [INDENT](../../com.aspose.cells/stylemodifyflag\#INDENT), [SHRINK\_TO\_FIT](../../com.aspose.cells/stylemodifyflag\#SHRINK-TO-FIT), [TEXT\_DIRECTION](../../com.aspose.cells/stylemodifyflag\#TEXT-DIRECTION), [RELATIVE\_INDENT](../../com.aspose.cells/stylemodifyflag\#RELATIVE-INDENT)) have been modified. |
| [ALL](#ALL) | All properties that can be modified for the style. |
| [BACKGROUND_COLOR](#BACKGROUND-COLOR) | Indicates whether background color has been modified. |
| [BORDERS](#BORDERS) | Indicates whether one or more borders([BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER), [BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER), [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER), [BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER), [DIAGONAL](../../com.aspose.cells/stylemodifyflag\#DIAGONAL), [HORIZONTAL\_BORDER](../../com.aspose.cells/stylemodifyflag\#HORIZONTAL-BORDER), [VERTICAL\_BORDER](../../com.aspose.cells/stylemodifyflag\#VERTICAL-BORDER)) have been modified for the style. |
| [BOTTOM_BORDER](#BOTTOM-BORDER) | Indicates whether bottom border has been modified for the style. |
| [CELL_SHADING](#CELL-SHADING) | Indicates whether one or more shading-related properties([PATTERN](../../com.aspose.cells/stylemodifyflag\#PATTERN), [FOREGROUND\_COLOR](../../com.aspose.cells/stylemodifyflag\#FOREGROUND-COLOR), [BACKGROUND\_COLOR](../../com.aspose.cells/stylemodifyflag\#BACKGROUND-COLOR)) have been modified. |
| [DIAGONAL](#DIAGONAL) | Indicates diagonal borders: [DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) and [DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER). |
| [DIAGONAL_DOWN_BORDER](#DIAGONAL-DOWN-BORDER) | Indicates whether diagonal-down border has been modified for the style. |
| [DIAGONAL_UP_BORDER](#DIAGONAL-UP-BORDER) | Indicates whether diagonal-up border has been modified for the style. |
| [DYNAMIC_STYLE_BORDERS](#DYNAMIC-STYLE-BORDERS) | Indicates borders of dynamic style: [HORIZONTAL\_BORDER](../../com.aspose.cells/stylemodifyflag\#HORIZONTAL-BORDER) and [VERTICAL\_BORDER](../../com.aspose.cells/stylemodifyflag\#VERTICAL-BORDER). |
| [FONT](#FONT) | Indicates whether one or more properties have been modified for the font of the style. |
| [FONT_CAP](#FONT-CAP) | unused. |
| [FONT_CHARSET](#FONT-CHARSET) | Indicates whether charset of the font has been modified. |
| [FONT_COLOR](#FONT-COLOR) | Indicates whether font color has been modified. |
| [FONT_DIRTY](#FONT-DIRTY) | unused. |
| [FONT_EQUALIZE](#FONT-EQUALIZE) | unused. |
| [FONT_FAMILY](#FONT-FAMILY) | Indicates whether font family has been modified. |
| [FONT_ITALIC](#FONT-ITALIC) | Indicates whether italic property of font has been modified. |
| [FONT_KERNING](#FONT-KERNING) | unused. |
| [FONT_NAME](#FONT-NAME) | Indicates whether font name has been modified. |
| [FONT_SCHEME](#FONT-SCHEME) | unused. |
| [FONT_SCRIPT](#FONT-SCRIPT) | Indicates whether subscript or superscript property of font has been modified. |
| [FONT_SIZE](#FONT-SIZE) | Indicates whether font size has been modified. |
| [FONT_SPACING](#FONT-SPACING) | unused. |
| [FONT_SPELLING_ERROR](#FONT-SPELLING-ERROR) | unused. |
| [FONT_STRIKE](#FONT-STRIKE) | Indicates whether strike property font has been modified. |
| [FONT_UNDERLINE](#FONT-UNDERLINE) | Indicates whether underline property of font has been modified. |
| [FONT_U_FILL_TX](#FONT-U-FILL-TX) | unused. |
| [FONT_VERTICAL_TEXT](#FONT-VERTICAL-TEXT) |  |
| [FONT_WEIGHT](#FONT-WEIGHT) | Indicates whether font weight has been modified. |
| [FOREGROUND_COLOR](#FOREGROUND-COLOR) | Indicates whether foreground color has been modified. |
| [HIDE_FORMULA](#HIDE-FORMULA) | Indicates whether hide formula has been modified. |
| [HORIZONTAL_ALIGNMENT](#HORIZONTAL-ALIGNMENT) | Indicates whether horizontal alignment has been modified. |
| [HORIZONTAL_BORDER](#HORIZONTAL-BORDER) | Indicates whether horizontal border has been modified for the style. |
| [INDENT](#INDENT) | Indicates whether indent property has been modified. |
| [LEFT_BORDER](#LEFT-BORDER) | Indicates whether left border has been modified for the style. |
| [LOCKED](#LOCKED) | Indicates whether locked property has been modified. |
| [NONE](#NONE) | No property has been specified. |
| [NUMBER_FORMAT](#NUMBER-FORMAT) | Indicates whether numberformat has been modified. |
| [PATTERN](#PATTERN) | Indicates whether pattern of the shading has been modified. |
| [PROTECTION_SETTINGS](#PROTECTION-SETTINGS) | Indicates whether one or more protection-related properties([LOCKED](../../com.aspose.cells/stylemodifyflag\#LOCKED), [HIDE\_FORMULA](../../com.aspose.cells/stylemodifyflag\#HIDE-FORMULA)) have been modified. |
| [RELATIVE_INDENT](#RELATIVE-INDENT) | Indicates whether relative indent property has been modified for the style. |
| [RIGHT_BORDER](#RIGHT-BORDER) | Indicates whether right border has been modified for the style. |
| [ROTATION](#ROTATION) | Indicates whether rotation property has been modified. |
| [SHRINK_TO_FIT](#SHRINK-TO-FIT) | Indicates whether shrink to fit property has been modified. |
| [SIDE_BORDERS](#SIDE-BORDERS) | Indicates the four side borders: [BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER), [BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER), [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER) and [BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER). |
| [TEXT_DIRECTION](#TEXT-DIRECTION) | Indicates whether text direction property has been modified. |
| [TOP_BORDER](#TOP-BORDER) | Indicates whether top border has been modified for the style. |
| [VERTICAL_ALIGNMENT](#VERTICAL-ALIGNMENT) | Indicates whether vertical alignment has been modified. |
| [VERTICAL_BORDER](#VERTICAL-BORDER) | Indicates whether vertical border has been modified for the style. |
| [WRAP_TEXT](#WRAP-TEXT) | Indicates whether wrap text property has been modified. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALIGNMENT_SETTINGS {#ALIGNMENT-SETTINGS}
```
public static final int ALIGNMENT_SETTINGS
```
Indicates whether one or more alignment-related properties([HORIZONTAL\_ALIGNMENT](../../com.aspose.cells/stylemodifyflag\#HORIZONTAL-ALIGNMENT), [VERTICAL\_ALIGNMENT](../../com.aspose.cells/stylemodifyflag\#VERTICAL-ALIGNMENT), [ROTATION](../../com.aspose.cells/stylemodifyflag\#ROTATION), [WRAP\_TEXT](../../com.aspose.cells/stylemodifyflag\#WRAP-TEXT), [WRAP\_TEXT](../../com.aspose.cells/stylemodifyflag\#WRAP-TEXT), [INDENT](../../com.aspose.cells/stylemodifyflag\#INDENT), [SHRINK\_TO\_FIT](../../com.aspose.cells/stylemodifyflag\#SHRINK-TO-FIT), [TEXT\_DIRECTION](../../com.aspose.cells/stylemodifyflag\#TEXT-DIRECTION), [RELATIVE\_INDENT](../../com.aspose.cells/stylemodifyflag\#RELATIVE-INDENT)) have been modified.
### ALL {#ALL}
```
public static final int ALL
```
All properties that can be modified for the style.
### BACKGROUND_COLOR {#BACKGROUND-COLOR}
```
public static final int BACKGROUND_COLOR
```
Indicates whether background color has been modified.
### BORDERS {#BORDERS}
```
public static final int BORDERS
```
Indicates whether one or more borders([BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER), [BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER), [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER), [BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER), [DIAGONAL](../../com.aspose.cells/stylemodifyflag\#DIAGONAL), [HORIZONTAL\_BORDER](../../com.aspose.cells/stylemodifyflag\#HORIZONTAL-BORDER), [VERTICAL\_BORDER](../../com.aspose.cells/stylemodifyflag\#VERTICAL-BORDER)) have been modified for the style.
### BOTTOM_BORDER {#BOTTOM-BORDER}
```
public static final int BOTTOM_BORDER
```
Indicates whether bottom border has been modified for the style.
### CELL_SHADING {#CELL-SHADING}
```
public static final int CELL_SHADING
```
Indicates whether one or more shading-related properties([PATTERN](../../com.aspose.cells/stylemodifyflag\#PATTERN), [FOREGROUND\_COLOR](../../com.aspose.cells/stylemodifyflag\#FOREGROUND-COLOR), [BACKGROUND\_COLOR](../../com.aspose.cells/stylemodifyflag\#BACKGROUND-COLOR)) have been modified.
### DIAGONAL {#DIAGONAL}
```
public static final int DIAGONAL
```
Indicates diagonal borders: [DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) and [DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER).
### DIAGONAL_DOWN_BORDER {#DIAGONAL-DOWN-BORDER}
```
public static final int DIAGONAL_DOWN_BORDER
```
Indicates whether diagonal-down border has been modified for the style.
### DIAGONAL_UP_BORDER {#DIAGONAL-UP-BORDER}
```
public static final int DIAGONAL_UP_BORDER
```
Indicates whether diagonal-up border has been modified for the style.
### DYNAMIC_STYLE_BORDERS {#DYNAMIC-STYLE-BORDERS}
```
public static final int DYNAMIC_STYLE_BORDERS
```
Indicates borders of dynamic style: [HORIZONTAL\_BORDER](../../com.aspose.cells/stylemodifyflag\#HORIZONTAL-BORDER) and [VERTICAL\_BORDER](../../com.aspose.cells/stylemodifyflag\#VERTICAL-BORDER).
### FONT {#FONT}
```
public static final int FONT
```
Indicates whether one or more properties have been modified for the font of the style.
### FONT_CAP {#FONT-CAP}
```
public static final int FONT_CAP
```
unused.
### FONT_CHARSET {#FONT-CHARSET}
```
public static final int FONT_CHARSET
```
Indicates whether charset of the font has been modified.
### FONT_COLOR {#FONT-COLOR}
```
public static final int FONT_COLOR
```
Indicates whether font color has been modified.
### FONT_DIRTY {#FONT-DIRTY}
```
public static final int FONT_DIRTY
```
unused.
### FONT_EQUALIZE {#FONT-EQUALIZE}
```
public static final int FONT_EQUALIZE
```
unused.
### FONT_FAMILY {#FONT-FAMILY}
```
public static final int FONT_FAMILY
```
Indicates whether font family has been modified.
### FONT_ITALIC {#FONT-ITALIC}
```
public static final int FONT_ITALIC
```
Indicates whether italic property of font has been modified.
### FONT_KERNING {#FONT-KERNING}
```
public static final int FONT_KERNING
```
unused.
### FONT_NAME {#FONT-NAME}
```
public static final int FONT_NAME
```
Indicates whether font name has been modified.
### FONT_SCHEME {#FONT-SCHEME}
```
public static final int FONT_SCHEME
```
unused.
### FONT_SCRIPT {#FONT-SCRIPT}
```
public static final int FONT_SCRIPT
```
Indicates whether subscript or superscript property of font has been modified.
### FONT_SIZE {#FONT-SIZE}
```
public static final int FONT_SIZE
```
Indicates whether font size has been modified.
### FONT_SPACING {#FONT-SPACING}
```
public static final int FONT_SPACING
```
unused.
### FONT_SPELLING_ERROR {#FONT-SPELLING-ERROR}
```
public static final int FONT_SPELLING_ERROR
```
unused.
### FONT_STRIKE {#FONT-STRIKE}
```
public static final int FONT_STRIKE
```
Indicates whether strike property font has been modified.
### FONT_UNDERLINE {#FONT-UNDERLINE}
```
public static final int FONT_UNDERLINE
```
Indicates whether underline property of font has been modified.
### FONT_U_FILL_TX {#FONT-U-FILL-TX}
```
public static final int FONT_U_FILL_TX
```
unused.
### FONT_VERTICAL_TEXT {#FONT-VERTICAL-TEXT}
```
public static final int FONT_VERTICAL_TEXT
```
### FONT_WEIGHT {#FONT-WEIGHT}
```
public static final int FONT_WEIGHT
```
Indicates whether font weight has been modified.
### FOREGROUND_COLOR {#FOREGROUND-COLOR}
```
public static final int FOREGROUND_COLOR
```
Indicates whether foreground color has been modified.
### HIDE_FORMULA {#HIDE-FORMULA}
```
public static final int HIDE_FORMULA
```
Indicates whether hide formula has been modified.
### HORIZONTAL_ALIGNMENT {#HORIZONTAL-ALIGNMENT}
```
public static final int HORIZONTAL_ALIGNMENT
```
Indicates whether horizontal alignment has been modified.
### HORIZONTAL_BORDER {#HORIZONTAL-BORDER}
```
public static final int HORIZONTAL_BORDER
```
Indicates whether horizontal border has been modified for the style. Only for dynamic style, such as conditional formatting.
### INDENT {#INDENT}
```
public static final int INDENT
```
Indicates whether indent property has been modified.
### LEFT_BORDER {#LEFT-BORDER}
```
public static final int LEFT_BORDER
```
Indicates whether left border has been modified for the style.
### LOCKED {#LOCKED}
```
public static final int LOCKED
```
Indicates whether locked property has been modified.
### NONE {#NONE}
```
public static final int NONE
```
No property has been specified.
### NUMBER_FORMAT {#NUMBER-FORMAT}
```
public static final int NUMBER_FORMAT
```
Indicates whether numberformat has been modified.
### PATTERN {#PATTERN}
```
public static final int PATTERN
```
Indicates whether pattern of the shading has been modified.
### PROTECTION_SETTINGS {#PROTECTION-SETTINGS}
```
public static final int PROTECTION_SETTINGS
```
Indicates whether one or more protection-related properties([LOCKED](../../com.aspose.cells/stylemodifyflag\#LOCKED), [HIDE\_FORMULA](../../com.aspose.cells/stylemodifyflag\#HIDE-FORMULA)) have been modified.
### RELATIVE_INDENT {#RELATIVE-INDENT}
```
public static final int RELATIVE_INDENT
```
Indicates whether relative indent property has been modified for the style. Only for dynamic style, such as conditional formatting.
### RIGHT_BORDER {#RIGHT-BORDER}
```
public static final int RIGHT_BORDER
```
Indicates whether right border has been modified for the style.
### ROTATION {#ROTATION}
```
public static final int ROTATION
```
Indicates whether rotation property has been modified.
### SHRINK_TO_FIT {#SHRINK-TO-FIT}
```
public static final int SHRINK_TO_FIT
```
Indicates whether shrink to fit property has been modified.
### SIDE_BORDERS {#SIDE-BORDERS}
```
public static final int SIDE_BORDERS
```
Indicates the four side borders: [BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER), [BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER), [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER) and [BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER).
### TEXT_DIRECTION {#TEXT-DIRECTION}
```
public static final int TEXT_DIRECTION
```
Indicates whether text direction property has been modified.
### TOP_BORDER {#TOP-BORDER}
```
public static final int TOP_BORDER
```
Indicates whether top border has been modified for the style.
### VERTICAL_ALIGNMENT {#VERTICAL-ALIGNMENT}
```
public static final int VERTICAL_ALIGNMENT
```
Indicates whether vertical alignment has been modified.
### VERTICAL_BORDER {#VERTICAL-BORDER}
```
public static final int VERTICAL_BORDER
```
Indicates whether vertical border has been modified for the style. Only for dynamic style, such as conditional formatting.
### WRAP_TEXT {#WRAP-TEXT}
```
public static final int WRAP_TEXT
```
Indicates whether wrap text property has been modified.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
