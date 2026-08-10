---
title: "Workbook Class"
linktitle: "Workbook"
articleTitle: "Workbook"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a root object to create an Excel spreadsheet."
type: docs
weight: 7540
url: /python-java/asposecells.api/workbook/
---

## Workbook class

Represents a root object to create an Excel spreadsheet.

## Constructors

| Name | Description |
| --- | --- |
| [Workbook](#constructor) | Initializes a new instance of the Workbook class. The default file format type is Xlsx. If you want to create other type |
| [Workbook](#constructor) | Initializes a new instance of the Workbook class. The default file format type is Excel97To2003. |
| [Workbook](#constructor) |  |
| [Workbook](#constructor) | Initializes a new instance of the Workbook class and open a file. |
| [Workbook](#constructor) | Initializes a new instance of the Workbook class and open a file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Settings](#settings) | WorkbookSettings | Represents the workbook settings. |
| [Worksheets](#worksheets) | WorksheetCollection | Gets the WorksheetCollection collection in the spreadsheet. |
| [IsLicensed](#islicensed) | boolean | Indicates whether license is set. |
| [Colors](#colors) | Color[] | Returns colors in the palette for the spreadsheet. The palette has 56 entries, each represented by an RGB value. |
| [CountOfStylesInPool](#countofstylesinpool) | int | Gets number of the styles in the style pool. |
| [DefaultStyle](#defaultstyle) | Style | Gets or sets the default Style object of the workbook. The DefaultStyle property is useful to implement a Style for the  |
| [IsDigitallySigned](#isdigitallysigned) | boolean | Indicates if this spreadsheet is digitally signed. |
| [IsWorkbookProtectedWithPassword](#isworkbookprotectedwithpassword) | boolean | Indicates whether structure or window is protected with password. |
| [VbaProject](#vbaproject) | VbaProject | Gets the VbaProject in a spreadsheet. |
| [HasMacro](#hasmacro) | boolean | Indicates if this spreadsheet contains macro/VBA. |
| [HasRevisions](#hasrevisions) | boolean | Gets if the workbook has any tracked changes |
| [FileName](#filename) | String | Gets and sets the current file name. If the file is opened by stream and there are some external formula references, ple |
| [CellsDataTableFactory](#cellsdatatablefactory) | CellsDataTableFactory | Gets the factory for building ICellsDataTable from custom objects |
| [DataSorter](#datasorter) | DataSorter | Gets a DataSorter object to sort data. |
| [Theme](#theme) | String | Gets the theme name. |
| [BuiltInDocumentProperties](#builtindocumentproperties) | BuiltInDocumentPropertyCollection | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new pro |
| [CustomDocumentProperties](#customdocumentproperties) | CustomDocumentPropertyCollection | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [FileFormat](#fileformat) | int | Gets and sets the file format. The value of the property is FileFormatType integer constant. |
| [HasCustomFunction](#hascustomfunction) | boolean |  |
| [InterruptMonitor](#interruptmonitor) | AbstractInterruptMonitor | Gets and sets the interrupt monitor. |
| [ContentTypeProperties](#contenttypeproperties) | ContentTypePropertyCollection | Gets the list of ContentTypeProperty objects in the workbook. |
| [CustomXmlParts](#customxmlparts) | CustomXmlPartCollection | Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [DataMashup](#datamashup) | DataMashup | Gets mashup data. |
| [RibbonXml](#ribbonxml) | String | Gets and sets the XML file that defines the Ribbon UI. |
| [AbsolutePath](#absolutepath) | String | Gets and sets the absolute path of the file. Only used for external links. |
| [DataConnections](#dataconnections) | ExternalConnectionCollection | Gets the ExternalConnection collection. |
| [DataModel](#datamodel) | DataModel |  |

## Methods

| Name | Description |
| --- | --- |
| [addDigitalSignature](#adddigitalsignature) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later).

Only support adding Xmldsig Digital Signatur |
| [getDigitalSignature](#getdigitalsignature) | Gets digital signature from file. |
| [removePersonalInformation](#removepersonalinformation) | Removes personal information. |
| [refreshAll](#refreshall) |  |
| [dispose](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [parseFormulas](#parseformulas) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [startAccessCache](#startaccesscache) | Starts the session that uses caches to access data.

If the cache of specified data access requires some data models in  |
| [closeAccessCache](#closeaccesscache) | Closes the session that uses caches to access data. |
| [save](#save) | Saves the workbook to the disk. |
| [removeUnusedStyles](#removeunusedstyles) | Remove all unused styles. |
| [createStyle](#createstyle) | Creates a new style. |
| [createBuiltinStyle](#createbuiltinstyle) | Creates built-in style by given type. |
| [createCellsColor](#createcellscolor) | Creates a CellsColor object. |
| [replace](#replace) | Replaces a cell's value with a new string. |
| [copy](#copy) | Copies another Workbook object.

It's very simple to clone an Excel file. |
| [combine](#combine) | Combines another Workbook object.

Merge Excel, ODS , CSV and other files to one file. |
| [getStyleInPool](#getstyleinpool) | Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple refere |
| [getFonts](#getfonts) | Gets all fonts in the style pool. |
| [getNamedStyle](#getnamedstyle) | Gets the named style in the style pool. |
| [mergeNamedStyles](#mergenamedstyles) |  |
| [changePalette](#changepalette) | Changes the palette for the spreadsheet in the specified index.

The palette has 56 entries, each represented by an RGB  |
| [isColorInPalette](#iscolorinpalette) | Checks if a color is in the palette for the spreadsheet. |
| [calculateFormula](#calculateformula) | Calculates the result of formulas.

For all supported formulas, please see the list at https://docs.aspose.com/display/c |
| [refreshDynamicArrayFormulas](#refreshdynamicarrayformulas) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in  |
| [getMatchingColor](#getmatchingcolor) | Find best matching Color in current palette. |
| [setEncryptionOptions](#setencryptionoptions) | Set Encryption Options. |
| [protect](#protect) | Protects a workbook. |
| [protectSharedWorkbook](#protectsharedworkbook) | Protects a shared workbook. |
| [unprotect](#unprotect) | Unprotects a workbook. |
| [unprotectSharedWorkbook](#unprotectsharedworkbook) | Unprotects a shared workbook. |
| [removeMacro](#removemacro) | Removes VBA/macro from this spreadsheet. |
| [removeDigitalSignature](#removedigitalsignature) | Removes digital signature from this spreadsheet. |
| [acceptAllRevisions](#acceptallrevisions) | Accepts all tracked changes in the workbook. |
| [removeExternalLinks](#removeexternallinks) | Removes all external links in the workbook.

NOTE: This member is now obsolete. Instead, please use ExternalLinkCollecti |
| [getThemeColor](#getthemecolor) | Gets theme color. |
| [setThemeColor](#setthemecolor) | Sets the theme color |
| [customTheme](#customtheme) | Customs the theme.

The length of colors should be 12. Array index Theme type 0 Backgournd1 1 Text1 2 Backgournd2 3 Text |
| [copyTheme](#copytheme) | Copies the theme from another workbook. |
| [hasExernalLinks](#hasexernallinks) | Indicates whether this workbook contains external links to other data sources.

NOTE: This member is now obsolete. Inste |
| [updateCustomFunctionDefinition](#updatecustomfunctiondefinition) | Updates definition of custom functions.

This method can be used for some special scenarios. For example, if user needs  |
| [updateLinkedDataSource](#updatelinkeddatasource) | If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data fro |
| [importXml](#importxml) | Imports/Updates an XML data file into the workbook. |
| [exportXml](#exportxml) | Export XML data linked by the specified XML map. |
| [setDigitalSignature](#setdigitalsignature) | Sets digital signature to an spreadsheet file (Excel2007 and later).

Only support adding Xmldsig Digital Signature |
| [createWorkbookFromBytes](#createworkbookfrombytes) | Initializes a new instance of the Workbook class and open a byte array. |
| [saveToBytes](#savetobytes) | Save the workbook to a byte array. |

### Workbook() (1 of 5) {#constructor}

Initializes a new instance of the Workbook class. The default file format type is Xlsx. If you want to create other types of files, please use Workbook(FileFormatType).

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

workbook = Workbook()
```

---

### Workbook(fileFormatType) (2 of 5) {#constructor-1}

Initializes a new instance of the Workbook class. The default file format type is Excel97To2003.

| Parameter | Type | Description |
| --- | --- | --- |
| fileFormatType | int | A FileFormatType value. The new file format. |

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

workbook = Workbook(FileFormatType.XLSX)
```

---

### Workbook(loadOptions) (3 of 5) {#constructor-2}

---

### Workbook(file) (4 of 5) {#constructor-3}

Initializes a new instance of the Workbook class and open a file.

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The file name. |

---

### Workbook(file, loadOptions) (5 of 5) {#constructor-4}

Initializes a new instance of the Workbook class and open a file.

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The file name. |
| loadOptions | LoadOptions | The load options |

### Workbook.Settings property {#settings}

Represents the workbook settings.

**Type:** WorkbookSettings

### Workbook.Worksheets property {#worksheets}

Gets the WorksheetCollection collection in the spreadsheet.

**Type:** WorksheetCollection

### Workbook.IsLicensed property {#islicensed}

Indicates whether license is set.

**Type:** boolean

### Workbook.Colors property {#colors}

Returns colors in the palette for the spreadsheet. The palette has 56 entries, each represented by an RGB value.

**Type:** Color[]

### Workbook.CountOfStylesInPool property {#countofstylesinpool}

Gets number of the styles in the style pool.

**Type:** int

### Workbook.DefaultStyle property {#defaultstyle}

Gets or sets the default Style object of the workbook. The DefaultStyle property is useful to implement a Style for the whole Workbook.

**Type:** Style

### Workbook.IsDigitallySigned property {#isdigitallysigned}

Indicates if this spreadsheet is digitally signed.

**Type:** boolean

### Workbook.IsWorkbookProtectedWithPassword property {#isworkbookprotectedwithpassword}

Indicates whether structure or window is protected with password.

**Type:** boolean

### Workbook.VbaProject property {#vbaproject}

Gets the VbaProject in a spreadsheet.

**Type:** VbaProject

### Workbook.HasMacro property {#hasmacro}

Indicates if this spreadsheet contains macro/VBA.

**Type:** boolean

### Workbook.HasRevisions property {#hasrevisions}

Gets if the workbook has any tracked changes

**Type:** boolean

### Workbook.FileName property {#filename}

Gets and sets the current file name. If the file is opened by stream and there are some external formula references, please set the file name.

**Type:** String

### Workbook.CellsDataTableFactory property {#cellsdatatablefactory}

Gets the factory for building ICellsDataTable from custom objects

**Type:** CellsDataTableFactory

### Workbook.DataSorter property {#datasorter}

Gets a DataSorter object to sort data.

**Type:** DataSorter

### Workbook.Theme property {#theme}

Gets the theme name.

**Type:** String

### Workbook.BuiltInDocumentProperties property {#builtindocumentproperties}

Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list: Title Subject Author Keywords Comments Template Last Author Revision Number Application Name Last Print Date Creation Date Last Save Time Total Editing Time Number of Pages Number of Words Number of Characters Security Category Format Manager Company Number of Bytes Number of Lines Number of Paragraphs Number of Slides Number of Notes Number of Hidden Slides Number of Multimedia Clips

**Type:** BuiltInDocumentPropertyCollection

### Workbook.CustomDocumentProperties property {#customdocumentproperties}

Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.

**Type:** CustomDocumentPropertyCollection

### Workbook.FileFormat property {#fileformat}

Gets and sets the file format. The value of the property is FileFormatType integer constant.

**Type:** int

### Workbook.HasCustomFunction property {#hascustomfunction}

**Type:** boolean

### Workbook.InterruptMonitor property {#interruptmonitor}

Gets and sets the interrupt monitor.

**Type:** AbstractInterruptMonitor

### Workbook.ContentTypeProperties property {#contenttypeproperties}

Gets the list of ContentTypeProperty objects in the workbook.

**Type:** ContentTypePropertyCollection

### Workbook.CustomXmlParts property {#customxmlparts}

Represents a Custom XML Data Storage Part (custom XML data within a package).

**Type:** CustomXmlPartCollection

### Workbook.DataMashup property {#datamashup}

Gets mashup data.

**Type:** DataMashup

### Workbook.RibbonXml property {#ribbonxml}

Gets and sets the XML file that defines the Ribbon UI.

**Type:** String

### Workbook.AbsolutePath property {#absolutepath}

Gets and sets the absolute path of the file. Only used for external links.

**Type:** String

### Workbook.DataConnections property {#dataconnections}

Gets the ExternalConnection collection.

**Type:** ExternalConnectionCollection

### Workbook.DataModel property {#datamodel}

**Type:** DataModel

### addDigitalSignature(digitalSignatureCollection) {#adddigitalsignature}

Adds digital signature to an OOXML spreadsheet file (Excel2007 and later).

Only support adding Xmldsig Digital Signature to an OOXML spreadsheet file

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### getDigitalSignature() {#getdigitalsignature}

Gets digital signature from file.

### removePersonalInformation() {#removepersonalinformation}

Removes personal information.

### refreshAll() {#refreshall}

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### parseFormulas(ignoreError) {#parseformulas}

Parses all formulas which have not been parsed when they were loaded from template file or set to a cell.

| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Whether ignore error for invalid formula. For one invalid formula, if ignore error then this formula will be ignored and the process will continue to parse other formulas, otherwise exception will be thrown. |

### startAccessCache(opts) {#startaccesscache}

Starts the session that uses caches to access data.

If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them. After finishing the access to the data, closeAccessCache(int) should be invoked with same options to clear all caches and recover normal access mode.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | int | A AccessCacheOptions value. options of data access |

### closeAccessCache(opts) {#closeaccesscache}

Closes the session that uses caches to access data.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | int | A AccessCacheOptions value. options of data access |

### save(fileName, saveFormat) (1 of 3) {#save}

Saves the workbook to the disk.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveFormat | int | A SaveFormat value. The save format type. |

**Example:**

```python
workbook = Workbook()
sheets = workbook.getWorksheets()
cells = sheets.get(0).getCells()
cells.get("A1").putValue("Hello world!")
workbook.save("Book1.xls", SaveFormat.EXCEL_97_TO_2003)
```

---

### save(fileName) (2 of 3) {#save-1}

Save the workbook to the disk.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String |  |

---

### save(fileName, saveOptions) (3 of 3) {#save-2}

Saves the workbook to the disk.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveOptions | SaveOptions | The save options. |

### removeUnusedStyles() {#removeunusedstyles}

Remove all unused styles.

### createStyle() (1 of 2) {#createstyle}

Creates a new style.

**Returns:** Returns a style object.

---

### createStyle(cloneDefaultStyle) (2 of 2) {#createstyle-1}

### createBuiltinStyle(type) {#createbuiltinstyle}

Creates built-in style by given type.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A BuiltinStyleType value. The builtin style stype. |

**Returns:** Style object

### createCellsColor() {#createcellscolor}

Creates a CellsColor object.

**Returns:** Returns a CellsColor object.

### replace(placeHolder, newValue) (1 of 5) {#replace}

Replaces a cell's value with a new string.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |

**Example:**

```python
workbook = Workbook()
workbook.replace("AnOldValue", "NewValue")
```

---

### replace(placeHolder, newValue) (2 of 5) {#replace-1}

Replaces a cell's value with a new integer.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | int | Integer value to replace |

**Example:**

```python
workbook = Workbook()
newValue = 100
workbook.replace("AnOldValue", newValue)
```

---

### replace(placeHolder, newValue) (3 of 5) {#replace-2}

Replaces a cell's value with a new double.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | float | Double value to replace |

**Example:**

```python
workbook = Workbook()
newValue = 100.0
workbook.replace("AnOldValue", newValue)
```

---

### replace(placeHolder, newValues, isVertical) (4 of 5) {#replace-3}

Replaces a cell's value with a new string array.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | String[] | String array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

workbook = Workbook("Book2.xlsx")
workbook.replace("OldString", ["Tom", "Alice", "Jerry"], True)
```

---

### replace(placeHolder, newValue, options) (5 of 5) {#replace-4}

Replaces a cell's value with a new string.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
| options | ReplaceOptions | The replace options |

### copy(source, copyOptions) (1 of 2) {#copy}

Copies another Workbook object.

It's very simple to clone an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |
| copyOptions | CopyOptions | The options of copying other workbook. |

---

### copy(source) (2 of 2) {#copy-1}

Copies data from a source Workbook object.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |

### combine(secondWorkbook) {#combine}

Combines another Workbook object.

Merge Excel, ODS , CSV and other files to one file.

| Parameter | Type | Description |
| --- | --- | --- |
| secondWorkbook | Workbook | Another Workbook object. |

### getStyleInPool(index) {#getstyleinpool}

Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells.

If the returned style is changed, the style of all cells(which refers to this style) will be changed.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |

**Returns:** The style in the pool corresponds to given index, may be null.

### getFonts() {#getfonts}

Gets all fonts in the style pool.

### getNamedStyle(name) {#getnamedstyle}

Gets the named style in the style pool.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | name of the style |

**Returns:** named style, maybe null.

### mergeNamedStyles(source) {#mergenamedstyles}

### changePalette(color, index) {#changepalette}

Changes the palette for the spreadsheet in the specified index.

The palette has 56 entries, each represented by an RGB value. If you set a color which is not in the palette, it will not take effect. So if you want to set a custom color, please change the palette at first. The following is the standard color palette. Color Red Green Blue Black 0 0 0 White 255 255 255 Red 255 0 0 Lime 0 255 0 Blue 0 0 255 Yellow 255 255 0 Magenta 255 0 255 Cyan 0 255 255 Maroon 128 0 0 Green 0 128 0 Navy 0 0 128 Olive 128 128 0 Purple 128 0 128 Teal 0 128 128 Silver 192 192 192 Gray 128 128 128 Color17 153 153 255 Color18 153 51 102 Color19 255 255 204 Color20 204 255 255 Color21 102 0 102 Color22 255 128 128 Color23 0 102 204 Color24 204 204 255 Color25 0 0 128 Color26 255 0 255 Color27 255 255 0 Color28 0 255 255 Color29 128 0 128 Color30 128 0 0 Color31 0 128 128 Color32 0 0 255 Color33 0 204 255 Color34 204 255 255 Color35 204 255 204 Color36 255 255 153 Color37 153 204 255 Color38 255 153 204 Color39 204 153 255 Color40 255 204 153 Color41 51 102 255 Color42 51 204 204 Color43 153 204 0 Color44 255 204 0 Color45 255 153 0 Color46 255 102 0 Color47 102 102 153 Color48 150 150 150 Color49 0 51 102 Color50 51 153 102 Color51 0 51 0 Color52 51 51 0 Color53 153 51 0 Color54 153 51 102 Color55 51 51 153 Color56 51 51 51

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | Color structure. |
| index | int | Palette index, 0 - 55. |

### isColorInPalette(color) {#iscolorinpalette}

Checks if a color is in the palette for the spreadsheet.

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | Color structure. |

**Returns:** Returns true if this color is in the palette. Otherwise, returns false

### calculateFormula() (1 of 3) {#calculateformula}

Calculates the result of formulas.

For all supported formulas, please see the list at https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

---

### calculateFormula(ignoreError) (2 of 3) {#calculateformula-1}

Calculates the result of formulas.

| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |

---

### calculateFormula(options) (3 of 3) {#calculateformula-2}

Calculating formulas in this workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |

### refreshDynamicArrayFormulas(calculate) (1 of 2) {#refreshdynamicarrayformulas}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.

| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |

---

### refreshDynamicArrayFormulas(calculate, copts) (2 of 2) {#refreshdynamicarrayformulas-1}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)

For performance consideration, we do not refresh all dynamic array formulas automatically when the formula itself or the data it references to changed. So user need to call this method manually after those operations which may influence dynamic array formulas, such as importing/setting cell values, inserting/deleting rows/columns/ranges, ...etc. For most formulas with functions, calculating the spill range also needs to calculating the formula, so in general true value for "calculate" flag is preferred. If the formula is simple, such as a range reference or array(for example "=C1:E5", "={1,2;3,4}", ...), simple function on a range or array(for example "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), and all formulas will be calculated later(such as by calculateFormula(com.aspose.cells.CalculationOptions) ), then using false vlaue for "calculate" flag may avoid the duplicated calculation for the benefit of performance.

| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |
| copts | CalculationOptions | The options for calculating formulas |

### getMatchingColor(rawColor) {#getmatchingcolor}

Find best matching Color in current palette.

| Parameter | Type | Description |
| --- | --- | --- |
| rawColor | Color | Raw color. |

**Returns:** Best matching color.

### setEncryptionOptions(encryptionType, keyLength) {#setencryptionoptions}

Set Encryption Options.

| Parameter | Type | Description |
| --- | --- | --- |
| encryptionType | int | A EncryptionType value. The encryption type. |
| keyLength | int | The key length. |

### protect(protectionType, password) {#protect}

Protects a workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| protectionType | int | A ProtectionType value. Protection type. |
| password | String | Password to protect the workbook. |

### protectSharedWorkbook(password) {#protectsharedworkbook}

Protects a shared workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to protect the workbook. |

### unprotect(password) {#unprotect}

Unprotects a workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to unprotect the workbook. |

### unprotectSharedWorkbook(password) {#unprotectsharedworkbook}

Unprotects a shared workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to unprotect the workbook. |

### removeMacro() {#removemacro}

Removes VBA/macro from this spreadsheet.

### removeDigitalSignature() {#removedigitalsignature}

Removes digital signature from this spreadsheet.

### acceptAllRevisions() {#acceptallrevisions}

Accepts all tracked changes in the workbook.

### removeExternalLinks() {#removeexternallinks}

Removes all external links in the workbook.

NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Clear() method. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

### getThemeColor(type) {#getthemecolor}

Gets theme color.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ThemeColorType value. The theme color type. |

**Returns:** The theme color.

### setThemeColor(type, color) {#setthemecolor}

Sets the theme color

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A ThemeColorType value. The theme color type. |
| color | Color | the theme color |

### customTheme(themeName, colors) {#customtheme}

Customs the theme.

The length of colors should be 12. Array index Theme type 0 Backgournd1 1 Text1 2 Backgournd2 3 Text2 4 Accent1 5 Accent2 6 Accent3 7 Accent4 8 Accent5 9 Accent6 10 Hyperlink 11 Followed Hyperlink

| Parameter | Type | Description |
| --- | --- | --- |
| themeName | String | The theme name |
| colors | Color[] | The theme colors |

### copyTheme(source) {#copytheme}

Copies the theme from another workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source workbook. |

### hasExernalLinks() {#hasexernallinks}

Indicates whether this workbook contains external links to other data sources.

NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Count to check whether there are external links in this workbook. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** Whether this workbook contains external links to other data sources.

### updateCustomFunctionDefinition(definition) {#updatecustomfunctiondefinition}

Updates definition of custom functions.

This method can be used for some special scenarios. For example, if user needs some parameters of some custom functions be calculated in array mode, then user may provide their own definition with implemented CustomFunctionDefinition.getArrayModeParameters(java.lang.String) for those functions. After the data of formulas being updated, those specified parameters will be calculated in array mode automatically when calculating corresponding custom functions.

| Parameter | Type | Description |
| --- | --- | --- |
| definition | CustomFunctionDefinition | Special definition of custom functions for user's special requirement. |

### updateLinkedDataSource(externalWorkbooks) {#updatelinkeddatasource}

If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources.

If corresponding external link cannot be found for one workbook, then this workbook will be ignored. So when you set a formula later with one new external link which you intend to make the ignored workbook be linked to it, the link cannot be performed until you call this this method again with those workbooks.

| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Workbooks that will be used to update data of external links referenced by this workbook. The match of those workbooks with external links is determined by FileName and ExternalLink.DataSource . So please make sure FileName has been specified with the proper value for every workbook so they can be linked to corresponding external link. |

### importXml(url, sheetName, row, col) (1 of 2) {#importxml}

Imports/Updates an XML data file into the workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| url | String | the url/path of the xml file. |
| sheetName | String | the destination sheet name. |
| row | int | the destination row |
| col | int | the destination column |

---

### importXml(stream, sheetName, row, col) (2 of 2) {#importxml-1}

Imports/Updates an XML data file into the workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | InputStream | the xml file stream. |
| sheetName | String | the destination sheet name. |
| row | int | the destination row. |
| col | int | the destination column. |

### exportXml(mapName, path) (1 of 2) {#exportxml}

Export XML data linked by the specified XML map.

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| path | String | the export path |

---

### exportXml(mapName, stream) (2 of 2) {#exportxml-1}

Export XML data linked by the specified XML map.

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| stream | OutputStream | the export stream |

### setDigitalSignature(digitalSignatureCollection) {#setdigitalsignature}

Sets digital signature to an spreadsheet file (Excel2007 and later).

Only support adding Xmldsig Digital Signature

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### createWorkbookFromBytes(byte_array) (1 of 2) {#createworkbookfrombytes}

Initializes a new instance of the Workbook class and open a byte array.

| Parameter | Type | Description |
| --- | --- | --- |
| byte_array | bytes | The byte array |

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

with open('Book2.xlsx', 'rb') as f:
    wb = Workbook.createWorkbookFromBytes(f.read())
    wb.save('result.xlsx')

jpype.shutdownJVM()
```

---

### createWorkbookFromBytes(byte_array, loadOptions) (2 of 2) {#createworkbookfrombytes-1}

Initializes a new instance of the Workbook class and open a byte array.

| Parameter | Type | Description |
| --- | --- | --- |
| byte_array | bytes | The byte array |
| loadOptions | LoadOptions | The load options |

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

loadOptions = LoadOptions()
with open('Book2.xlsx', 'rb') as f:
    wb = Workbook.createWorkbookFromBytes(f.read(), loadOptions=loadOptions)
    wb.save('result.xlsx')

jpype.shutdownJVM()
```

### saveToBytes(saveOptions) (1 of 2) {#savetobytes}

Save the workbook to a byte array.

| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | SaveOptions | The save options |

**Returns:** A byte array.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook("Book2.xlsx")
saveOptions = XlsSaveOptions()
with open("wb.xls", "wb") as w:
    byte_array = wb.saveToBytes(saveOptions)
    w.write(byte_array)

jpype.shutdownJVM()
```

---

### saveToBytes(saveFormat) (2 of 2) {#savetobytes-1}

Save the workbook to a byte array.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | The save file format type |

**Returns:** A byte array.

**Example:**

```python
import jpype
import asposecells
jpype.startJVM()
from asposecells.api import *

wb = Workbook("Book2.xlsx")
with open("wb.xlsx", "wb") as w:
    byte_array = wb.saveToBytes(SaveFormat.XLSX)
    w.write(byte_array)

jpype.shutdownJVM()
```
