##LoadDataFilterOptions
Represents the options to filter data when loading workbook from template.
**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```
Represents the options to filter data when loading workbook from template.
## Fields
| Field | Description |
| --- | --- |
| [ALL](#ALL) | Load all |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | Load settings for workbook |
| [CELL_BLANK](#CELL-BLANK) | Load cells whose value is blank |
| [CELL_BOOL](#CELL-BOOL) | Load cells whose value is bool |
| [CELL_DATA](#CELL-DATA) | Load cells data including values, formulas and formatting |
| [CELL_ERROR](#CELL-ERROR) | Load cells whose value is error |
| [CELL_NUMERIC](#CELL-NUMERIC) | Load cells whose value is numeric(including datetime) |
| [CELL_STRING](#CELL-STRING) | Load cells whose value is string |
| [CELL_VALUE](#CELL-VALUE) | Load cells value(all value types) only |
| [CHART](#CHART) | Load charts |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Load conditional formatting |
| [DATA_VALIDATION](#DATA-VALIDATION) | Load data validations |
| [DEFINED_NAMES](#DEFINED-NAMES) | Load defined Name objects |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | Load document properties |
| [DRAWING](#DRAWING) | Drawing objects(including Chart, Picture, OleObject and all other drawing objects) |
| [FORMULA](#FORMULA) | Load cell formulas. |
| [HYPERLINKS](#HYPERLINKS) | Load hyperlinks |
| [MERGED_AREA](#MERGED-AREA) | Load merged cells |
| [NONE](#NONE) | Load nothing for sheet data |
| [OLE_OBJECT](#OLE-OBJECT) | Load OleObjects |
| [PICTURE](#PICTURE) | Load pictures |
| [PIVOT_TABLE](#PIVOT-TABLE) | Load pivot tables |
| [REVISION](#REVISION) | Load revision logs |
| [SETTINGS](#SETTINGS) | Load settings for workbook and worksheet |
| [SHAPE](#SHAPE) | Load shapes |
| [SHEET_DATA](#SHEET-DATA) | Load all data of worksheet, such as cells data, settings, objects, ...etc. |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | Load settings for worksheet |
| [STRUCTURE](#STRUCTURE) | Load structure of the workbook |
| [STYLE](#STYLE) | Load styles for cell formatting |
| [TABLE](#TABLE) | Load tables |
| [VBA](#VBA) | Load VBA projects |
| [XML_MAP](#XML-MAP) | Load XmlMap |
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
### ALL {#ALL}
```
public static final int ALL
```
Load all
### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```
Load settings for workbook
### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```
Load cells whose value is blank
### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```
Load cells whose value is bool
### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```
Load cells data including values, formulas and formatting
### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```
Load cells whose value is error
### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```
Load cells whose value is numeric(including datetime)
### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```
Load cells whose value is string
### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```
Load cells value(all value types) only
### CHART {#CHART}
```
public static final int CHART
```
Load charts
### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```
Load conditional formatting
### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```
Load data validations
### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```
Load defined Name objects
### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```
Load document properties
### DRAWING {#DRAWING}
```
public static final int DRAWING
```
Drawing objects(including Chart, Picture, OleObject and all other drawing objects)
### FORMULA {#FORMULA}
```
public static final int FORMULA
```
Load cell formulas.
**Remarks**
Generally defined Name objects(DefinedNames) also need to be loaded when loading formulas because they may be referenced by formulas. So Formula or CellData option should work with DefinedNames option together(Formula\|DefinedNames or CellData\|DefinedNames) for most scenarios.
### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```
Load hyperlinks
### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```
Load merged cells
### NONE {#NONE}
```
public static final int NONE
```
Load nothing for sheet data
**Remarks**
NOTE: This member is now obsolete and please use Structure instead. This property will be removed 12 months later since December 2017. Aspose apologizes for any inconvenience you may have experienced.
### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```
Load OleObjects
### PICTURE {#PICTURE}
```
public static final int PICTURE
```
Load pictures
### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```
Load pivot tables
### REVISION {#REVISION}
```
public static final int REVISION
```
Load revision logs
### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```
Load settings for workbook and worksheet
### SHAPE {#SHAPE}
```
public static final int SHAPE
```
Load shapes
**Remarks**
NOTE: This member is now obsolete and please use Drawing instead. This property will be removed 12 months later since November 2019. Aspose apologizes for any inconvenience you may have experienced.
### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```
Load all data of worksheet, such as cells data, settings, objects, ...etc.
### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```
Load settings for worksheet
### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```
Load structure of the workbook
### STYLE {#STYLE}
```
public static final int STYLE
```
Load styles for cell formatting
### TABLE {#TABLE}
```
public static final int TABLE
```
Load tables
### VBA {#VBA}
```
public static final int VBA
```
Load VBA projects
### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```
Load XmlMap
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
