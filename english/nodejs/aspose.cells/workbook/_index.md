---
title: "Workbook"
linktitle: "Workbook"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a root object to create an Excel spreadsheet."
type: docs
weight: 4670
url: /nodejs/aspose.cells/workbook/
---

## Workbook class

Represents a root object to create an Excel spreadsheet. The Workbook class denotes an Excel spreadsheet. Each spreadsheet can contain multiple worksheets. The basic feature of the class is to open and save native excel files. The class has some advanced features like copying data from other Workbooks, combining two Workbooks, converting Excel to PDF, rendering Excel to image and protecting the Excel spreadsheet.

```js
new Workbook()
```

Initializes a new instance of the Workbook class. The default file format type is Xlsx. If you want to create other types of files, please use Workbook(FileFormatType).

## Methods

| Name | Description |
| --- | --- |
| [acceptAllRevisions()](#acceptallrevisions) | Accepts all tracked changes in the workbook. |
| [addDigitalSignature(digitalSignatureCollection)](#adddigitalsignature) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). Only support adding Xmldsig Digital Signature |
| [calculateFormula()](#calculateformula) | Calculates the result of formulas. For all supported formulas, please see the list at https://docs.aspose.com/display/ce |
| [calculateFormula(ignoreError)](#calculateformula-1) | Calculates the result of formulas. |
| [calculateFormula(options)](#calculateformula-2) | Calculating formulas in this workbook. |
| [changePalette(color, index)](#changepalette) | Changes the palette for the spreadsheet in the specified index. The palette has 56 entries, each represented by an RGB v |
| [closeAccessCache(opts)](#closeaccesscache) | Closes the session that uses caches to access data. |
| [combine(secondWorkbook)](#combine) | Combines another Workbook object. Merge Excel, ODS , CSV and other files to one file. |
| [constructor_overload$1(fileFormatType)](#constructor-overload1) | Initializes a new instance of the Workbook class. The default file format type is Excel97To2003. |
| [constructor_overload$2()](#constructor-overload2) |  |
| [constructor_overload$3(file)](#constructor-overload3) | Initializes a new instance of the Workbook class and open a file. |
| [constructor_overload$4(file, loadOptions)](#constructor-overload4) | Initializes a new instance of the Workbook class and open a file. |
| [copy(source, copyOptions)](#copy) | Copies another Workbook object. It's very simple to clone an Excel file. |
| [copy(source)](#copy-1) | Copies data from a source Workbook object. |
| [copyTheme(source)](#copytheme) | Copies the theme from another workbook. |
| [createBuiltinStyle(type)](#createbuiltinstyle) | Creates built-in style by given type. |
| [createCellsColor()](#createcellscolor) | Creates a CellsColor object. |
| [createStyle()](#createstyle) | Creates a new style. |
| [createStyle()](#createstyle-1) |  |
| [customTheme(themeName, colors)](#customtheme) | Customs the theme. The length of colors should be 12. Array indexTheme type0Backgournd11Text12Backgournd23Text24Accent15 |
| [dispose()](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [exportXml(mapName, path)](#exportxml) | Export XML data linked by the specified XML map. |
| [exportXml(mapName, stream)](#exportxml-1) | Export XML data linked by the specified XML map. |
| [getAbsolutePath()](#getabsolutepath) | Gets and sets the absolute path of the file. Only used for external links. |
| [getBuiltInDocumentProperties()](#getbuiltindocumentproperties) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new pro |
| [getCellsDataTableFactory()](#getcellsdatatablefactory) | Gets the factory for building ICellsDataTable from custom objects |
| [getColors()](#getcolors) | Returns colors in the palette for the spreadsheet. The palette has 56 entries, each represented by an RGB value. |
| [getContentTypeProperties()](#getcontenttypeproperties) | Gets the list of ContentTypeProperty objects in the workbook. |
| [getCountOfStylesInPool()](#getcountofstylesinpool) | Gets number of the styles in the style pool. |
| [getCustomDocumentProperties()](#getcustomdocumentproperties) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [getCustomXmlParts()](#getcustomxmlparts) | Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [getDataConnections()](#getdataconnections) | Gets the ExternalConnection collection. |
| [getDataMashup()](#getdatamashup) | Gets mashup data. |
| [getDataModel()](#getdatamodel) |  |
| [getDataSorter()](#getdatasorter) | Gets a DataSorter object to sort data. |
| [getDefaultStyle()](#getdefaultstyle) | Gets or sets the default Style object of the workbook. The DefaultStyle property is useful to implement a Style for the  |
| [getDigitalSignature()](#getdigitalsignature) | Gets digital signature from file. |
| [getFileFormat()](#getfileformat) | Gets and sets the file format. The value of the property is FileFormatType integer constant. |
| [getFileName()](#getfilename) | Gets and sets the current file name. If the file is opened by stream and there are some external formula references, ple |
| [getFonts()](#getfonts) | Gets all fonts in the style pool. |
| [getInterruptMonitor()](#getinterruptmonitor) | Gets and sets the interrupt monitor. |
| [getMatchingColor(rawColor)](#getmatchingcolor) | Find best matching Color in current palette. |
| [getNamedStyle(name)](#getnamedstyle) | Gets the named style in the style pool. |
| [getRibbonXml()](#getribbonxml) | Gets and sets the XML file that defines the Ribbon UI. |
| [getSettings()](#getsettings) | Represents the workbook settings. |
| [getStyleInPool(index)](#getstyleinpool) | Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple refere |
| [getTheme()](#gettheme) | Gets the theme name. |
| [getThemeColor(type)](#getthemecolor) | Gets theme color. |
| [getVbaProject()](#getvbaproject) | Gets the VbaProject in a spreadsheet. |
| [getWorksheets()](#getworksheets) | Gets the WorksheetCollection collection in the spreadsheet. |
| [hasCustomFunction()](#hascustomfunction) |  |
| [hasExernalLinks()](#hasexernallinks) | Indicates whether this workbook contains external links to other data sources. NOTE: This member is now obsolete. Instea |
| [hasMacro()](#hasmacro) | Indicates if this spreadsheet contains macro/VBA. |
| [hasRevisions()](#hasrevisions) | Gets if the workbook has any tracked changes |
| [importXml(url, sheetName, row, col)](#importxml) | Imports/Updates an XML data file into the workbook. |
| [importXml(stream, sheetName, row, col)](#importxml-1) | Imports/Updates an XML data file into the workbook. |
| [isColorInPalette(color)](#iscolorinpalette) | Checks if a color is in the palette for the spreadsheet. |
| [isDigitallySigned()](#isdigitallysigned) | Indicates if this spreadsheet is digitally signed. |
| [isLicensed()](#islicensed) | Indicates whether license is set. |
| [isWorkbookProtectedWithPassword()](#isworkbookprotectedwithpassword) | Indicates whether structure or window is protected with password. |
| [mergeNamedStyles()](#mergenamedstyles) |  |
| [parseFormulas(ignoreError)](#parseformulas) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [protect(protectionType, password)](#protect) | Protects a workbook. |
| [protectSharedWorkbook(password)](#protectsharedworkbook) | Protects a shared workbook. |
| [refreshAll()](#refreshall) |  |
| [refreshDynamicArrayFormulas(calculate)](#refreshdynamicarrayformulas) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in  |
| [refreshDynamicArrayFormulas(calculate, copts)](#refreshdynamicarrayformulas-1) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) For performance co |
| [removeDigitalSignature()](#removedigitalsignature) | Removes digital signature from this spreadsheet. |
| [removeExternalLinks()](#removeexternallinks) | Removes all external links in the workbook. NOTE: This member is now obsolete. Instead, please use ExternalLinkCollectio |
| [removeMacro()](#removemacro) | Removes VBA/macro from this spreadsheet. |
| [removePersonalInformation()](#removepersonalinformation) | Removes personal information. |
| [removeUnusedStyles()](#removeunusedstyles) | Remove all unused styles. |
| [replace(placeHolder, newValue)](#replace) | Replaces a cell's value with a new string. |
| [replace(placeHolder, newValue)](#replace-1) | Replaces a cell's value with a new integer. |
| [replace(placeHolder, newValue)](#replace-2) | Replaces a cell's value with a new double. |
| [replace(placeHolder, newValues, isVertical)](#replace-3) | Replaces a cell's value with a new string array. |
| [replace(placeHolder, newValue, options)](#replace-4) | Replaces a cell's value with a new string. |
| [save(fileName, saveFormat)](#save) | Saves the workbook to the disk. |
| [save(fileName)](#save-1) | Save the workbook to the disk. |
| [save(fileName, saveOptions)](#save-2) | Saves the workbook to the disk. |
| [setAbsolutePath()](#setabsolutepath) | Gets and sets the absolute path of the file. Only used for external links. |
| [setDefaultStyle()](#setdefaultstyle) | Gets or sets the default Style object of the workbook. The DefaultStyle property is useful to implement a Style for the  |
| [setDigitalSignature(digitalSignatureCollection)](#setdigitalsignature) | Sets digital signature to an spreadsheet file (Excel2007 and later). Only support adding Xmldsig Digital Signature |
| [setEncryptionOptions(encryptionType, keyLength)](#setencryptionoptions) | Set Encryption Options. |
| [setFileFormat()](#setfileformat) | Gets and sets the file format. The value of the property is FileFormatType integer constant. |
| [setFileName()](#setfilename) | Gets and sets the current file name. If the file is opened by stream and there are some external formula references, ple |
| [setInterruptMonitor()](#setinterruptmonitor) | Gets and sets the interrupt monitor. |
| [setRibbonXml()](#setribbonxml) | Gets and sets the XML file that defines the Ribbon UI. |
| [setThemeColor(type, color)](#setthemecolor) | Sets the theme color |
| [startAccessCache(opts)](#startaccesscache) | Starts the session that uses caches to access data. If the cache of specified data access requires some data models in w |
| [unprotect(password)](#unprotect) | Unprotects a workbook. |
| [unprotectSharedWorkbook(password)](#unprotectsharedworkbook) | Unprotects a shared workbook. |
| [updateCustomFunctionDefinition(definition)](#updatecustomfunctiondefinition) | Updates definition of custom functions. This method can be used for some special scenarios. For example, if user needs s |
| [updateLinkedDataSource(externalWorkbooks)](#updatelinkeddatasource) | If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data fro |
| [createWorkbookFromStream(stream, callback)](#createworkbookfromstream) *(static)* | Initializes a new instance of the Workbook class and open a stream. |
| [createWorkbookFromStream(stream, loadOptions, callback)](#createworkbookfromstream-1) *(static)* | Initializes a new instance of the Workbook class and open a stream. |
| [save(workbook, stream, saveOptions)](#save-3) *(static)* | Save the workbook to the stream. |
| [save(workbook, stream, saveFormat)](#save-4) *(static)* | Save the workbook to the stream. |

### acceptAllRevisions() {#acceptallrevisions}

Accepts all tracked changes in the workbook.

### addDigitalSignature(digitalSignatureCollection) {#adddigitalsignature}

Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). Only support adding Xmldsig Digital Signature to an OOXML spreadsheet file

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### calculateFormula() {#calculateformula}

Calculates the result of formulas. For all supported formulas, please see the list at https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(ignoreError) {#calculateformula-1}

Calculates the result of formulas.

| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |

### calculateFormula(options) {#calculateformula-2}

Calculating formulas in this workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |

### changePalette(color, index) {#changepalette}

Changes the palette for the spreadsheet in the specified index. The palette has 56 entries, each represented by an RGB value.If you set a color which is not in the palette, it will not take effect.So if you want to set a custom color, please change the palette at first.The following is the standard color palette.ColorRedGreenBlueBlack000White255255255Red25500Lime02550Blue00255Yellow2552550Magenta2550255Cyan0255255Maroon12800Green01280Navy00128Olive1281280Purple1280128Teal0128128Silver192192192Gray128128128Color17153153255Color1815351102Color19255255204Color20204255255Color211020102Color22255128128Color230102204Color24204204255Color2500128Color262550255Color272552550Color280255255Color291280128Color3012800Color310128128Color3200255Color330204255Color34204255255Color35204255204Color36255255153Color37153204255Color38255153204Color39204153255Color40255204153Color4151102255Color4251204204Color431532040Color442552040Color452551530Color462551020Color47102102153Color48150150150Color49051102Color5051153102Color510510Color5251510Color53153510Color5415351102Color555151153Color56515151

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | Color structure. |
| index | Number | Palette index, 0 - 55. |

### closeAccessCache(opts) {#closeaccesscache}

Closes the session that uses caches to access data.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | Number | AccessCacheOptions |

### combine(secondWorkbook) {#combine}

Combines another Workbook object. Merge Excel, ODS , CSV and other files to one file.

| Parameter | Type | Description |
| --- | --- | --- |
| secondWorkbook | Workbook | Another Workbook object. |

### constructor_overload$1(fileFormatType) {#constructor-overload1}

Initializes a new instance of the Workbook class. The default file format type is Excel97To2003.

| Parameter | Type | Description |
| --- | --- | --- |
| fileFormatType | Number | FileFormatType |

### constructor_overload$2() {#constructor-overload2}

### constructor_overload$3(file) {#constructor-overload3}

Initializes a new instance of the Workbook class and open a file.

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The file name. |

### constructor_overload$4(file, loadOptions) {#constructor-overload4}

Initializes a new instance of the Workbook class and open a file.

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The file name. |
| loadOptions | LoadOptions | The load options |

### copy(source, copyOptions) {#copy}

Copies another Workbook object. It's very simple to clone an Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |
| copyOptions | CopyOptions | The options of copying other workbook. |

### copy(source) {#copy-1}

Copies data from a source Workbook object.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source Workbook object. |

### copyTheme(source) {#copytheme}

Copies the theme from another workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Workbook | Source workbook. |

### createBuiltinStyle(type) {#createbuiltinstyle}

Creates built-in style by given type.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | BuiltinStyleType |

**Returns:** Style — `Style` Style object

### createCellsColor() {#createcellscolor}

Creates a CellsColor object.

**Returns:** CellsColor — `CellsColor` Returns a CellsColor object.

### createStyle() {#createstyle}

Creates a new style.

**Returns:** Style — `Style` Returns a style object.

### createStyle() {#createstyle-1}

### customTheme(themeName, colors) {#customtheme}

Customs the theme. The length of colors should be 12. Array indexTheme type0Backgournd11Text12Backgournd23Text24Accent15Accent26Accent37Accent48Accent59Accent610Hyperlink11Followed Hyperlink

| Parameter | Type | Description |
| --- | --- | --- |
| themeName | String | The theme name |
| colors | Array ofColor | The theme colors |

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### exportXml(mapName, path) {#exportxml}

Export XML data linked by the specified XML map.

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| path | String | the export path |

### exportXml(mapName, stream) {#exportxml-1}

Export XML data linked by the specified XML map.

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of the XML map that need to be exported |
| stream | OutputStream | the export stream |

### getAbsolutePath() {#getabsolutepath}

Gets and sets the absolute path of the file. Only used for external links.

### getBuiltInDocumentProperties() {#getbuiltindocumentproperties}

Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list: TitleSubjectAuthorKeywordsCommentsTemplateLast AuthorRevision NumberApplication NameLast Print DateCreation DateLast Save TimeTotal Editing TimeNumber of PagesNumber of WordsNumber of CharactersSecurityCategoryFormatManagerCompanyNumber of BytesNumber of LinesNumber of ParagraphsNumber of SlidesNumber of NotesNumber of Hidden SlidesNumber of Multimedia Clips

**Example:**

```js
var doc = workbook.getBuiltInDocumentProperties().get("Author");
doc.setValue("John Smith");
```

### getCellsDataTableFactory() {#getcellsdatatablefactory}

Gets the factory for building ICellsDataTable from custom objects

### getColors() {#getcolors}

Returns colors in the palette for the spreadsheet. The palette has 56 entries, each represented by an RGB value.

### getContentTypeProperties() {#getcontenttypeproperties}

Gets the list of ContentTypeProperty objects in the workbook.

### getCountOfStylesInPool() {#getcountofstylesinpool}

Gets number of the styles in the style pool.

### getCustomDocumentProperties() {#getcustomdocumentproperties}

Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.

**Example:**

```js
var excel = new aspose.cells.Workbook();
excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

### getCustomXmlParts() {#getcustomxmlparts}

Represents a Custom XML Data Storage Part (custom XML data within a package).

### getDataConnections() {#getdataconnections}

Gets the ExternalConnection collection.

### getDataMashup() {#getdatamashup}

Gets mashup data.

### getDataModel() {#getdatamodel}

### getDataSorter() {#getdatasorter}

Gets a DataSorter object to sort data.

### getDefaultStyle() {#getdefaultstyle}

Gets or sets the default Style object of the workbook. The DefaultStyle property is useful to implement a Style for the whole Workbook.

### getDigitalSignature() {#getdigitalsignature}

Gets digital signature from file.

### getFileFormat() {#getfileformat}

Gets and sets the file format. The value of the property is FileFormatType integer constant.

### getFileName() {#getfilename}

Gets and sets the current file name. If the file is opened by stream and there are some external formula references, please set the file name.

### getFonts() {#getfonts}

Gets all fonts in the style pool.

### getInterruptMonitor() {#getinterruptmonitor}

Gets and sets the interrupt monitor.

### getMatchingColor(rawColor) {#getmatchingcolor}

Find best matching Color in current palette.

| Parameter | Type | Description |
| --- | --- | --- |
| rawColor | Color | Raw color. |

**Returns:** Color — `Color` Best matching color.

### getNamedStyle(name) {#getnamedstyle}

Gets the named style in the style pool.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | name of the style |

**Returns:** Style — `Style` named style, maybe null.

### getRibbonXml() {#getribbonxml}

Gets and sets the XML file that defines the Ribbon UI.

### getSettings() {#getsettings}

Represents the workbook settings.

### getStyleInPool(index) {#getstyleinpool}

Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells. If the returned style is changed, the style of all cells(which refers to this style) will be changed.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index. |

**Returns:** Style — `Style` The style in the pool corresponds to given index, may be null.

### getTheme() {#gettheme}

Gets the theme name.

### getThemeColor(type) {#getthemecolor}

Gets theme color.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ThemeColorType |

**Returns:** Color — `Color` The theme color.

### getVbaProject() {#getvbaproject}

Gets the VbaProject in a spreadsheet.

### getWorksheets() {#getworksheets}

Gets the WorksheetCollection collection in the spreadsheet.

**Returns:** WorksheetCollection — `WorksheetCollection` WorksheetCollection collection

### hasCustomFunction() {#hascustomfunction}

### hasExernalLinks() {#hasexernallinks}

Indicates whether this workbook contains external links to other data sources. NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Count to check whether there are external links in this workbook. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.@return {boolean} Whether this workbook contains external links to other data sources.

### hasMacro() {#hasmacro}

Indicates if this spreadsheet contains macro/VBA.

### hasRevisions() {#hasrevisions}

Gets if the workbook has any tracked changes

### importXml(url, sheetName, row, col) {#importxml}

Imports/Updates an XML data file into the workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| url | String | the url/path of the xml file. |
| sheetName | String | the destination sheet name. |
| row | Number | the destination row |
| col | Number | the destination column |

### importXml(stream, sheetName, row, col) {#importxml-1}

Imports/Updates an XML data file into the workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | InputStream | the xml file stream. |
| sheetName | String | the destination sheet name. |
| row | Number | the destination row. |
| col | Number | the destination column. |

### isColorInPalette(color) {#iscolorinpalette}

Checks if a color is in the palette for the spreadsheet.

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | Color structure. |

**Returns:** boolean — `boolean` Returns true if this color is in the palette. Otherwise, returns false

### isDigitallySigned() {#isdigitallysigned}

Indicates if this spreadsheet is digitally signed.

### isLicensed() {#islicensed}

Indicates whether license is set.

### isWorkbookProtectedWithPassword() {#isworkbookprotectedwithpassword}

Indicates whether structure or window is protected with password.

### mergeNamedStyles() {#mergenamedstyles}

### parseFormulas(ignoreError) {#parseformulas}

Parses all formulas which have not been parsed when they were loaded from template file or set to a cell.

| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Whether ignore error for invalid formula. For one invalid formula, if ignore error then this formula will be ignored and the process will continue to parse other formulas, otherwise exception will be thrown. |

### protect(protectionType, password) {#protect}

Protects a workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| protectionType | Number | ProtectionType |
| password | String | Password to protect the workbook. |

### protectSharedWorkbook(password) {#protectsharedworkbook}

Protects a shared workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to protect the workbook. |

### refreshAll() {#refreshall}

### refreshDynamicArrayFormulas(calculate) {#refreshdynamicarrayformulas}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.

| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |

### refreshDynamicArrayFormulas(calculate, copts) {#refreshdynamicarrayformulas-1}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) For performance consideration, we do not refresh all dynamic array formulas automatically when the formula itself or the data it references to changed. So user need to call this method manually after those operations which may influence dynamic array formulas, such as importing/setting cell values, inserting/deleting rows/columns/ranges, ...etc. For most formulas with functions, calculating the spill range also needs to calculating the formula, so in general true value for "calculate" flag is preferred. If the formula is simple, such as a range reference or array(for example "=C1:E5", "={1,2;3,4}", ...), simple function on a range or array(for example "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), and all formulas will be calculated later(such as by calculateFormula(com.aspose.cells.CalculationOptions)), then using false vlaue for "calculate" flag may avoid the duplicated calculation for the benefit of performance.

| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |
| copts | CalculationOptions | The options for calculating formulas |

### removeDigitalSignature() {#removedigitalsignature}

Removes digital signature from this spreadsheet.

### removeExternalLinks() {#removeexternallinks}

Removes all external links in the workbook. NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Clear() method. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

### removeMacro() {#removemacro}

Removes VBA/macro from this spreadsheet.

### removePersonalInformation() {#removepersonalinformation}

Removes personal information.

### removeUnusedStyles() {#removeunusedstyles}

Remove all unused styles.

### replace(placeHolder, newValue) {#replace}

Replaces a cell's value with a new string.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |

**Example:**

```js
var workbook = new aspose.cells.Workbook();
workbook.replace("AnOldValue", "NewValue");
```

### replace(placeHolder, newValue) {#replace-1}

Replaces a cell's value with a new integer.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | Number | Integer value to replace |

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var newValue = 100;
workbook.replace("AnOldValue", newValue);
```

### replace(placeHolder, newValue) {#replace-2}

Replaces a cell's value with a new double.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | Number | Double value to replace |

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var newValue = 100.0;
workbook.replace("AnOldValue", newValue);
```

### replace(placeHolder, newValues, isVertical) {#replace-3}

Replaces a cell's value with a new string array.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | Array of String | String array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var java = require("java");
var workbook = new aspose.cells.Workbook();
var newValues = java.newArray("java.lang.String", ["Tom", "Alice", "Jerry"]);
workbook.replace("AnOldValue", newValues, true);
```

### replace(placeHolder, newValue, options) {#replace-4}

Replaces a cell's value with a new string.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
| options | ReplaceOptions | The replace options |

### save(fileName, saveFormat) {#save}

Saves the workbook to the disk.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveFormat | Number | SaveFormat |

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var sheets = workbook.getWorksheets();
var cells = sheets.get(0).getCells();
cells.get("A1").putValue("Hello world!");
workbook.save("Book1.xls", aspose.cells.SaveFormat.EXCEL_97_TO_2003);
```

### save(fileName) {#save-1}

Save the workbook to the disk.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String |  |

### save(fileName, saveOptions) {#save-2}

Saves the workbook to the disk.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |
| saveOptions | SaveOptions | The save options. |

### setAbsolutePath() {#setabsolutepath}

Gets and sets the absolute path of the file. Only used for external links.

### setDefaultStyle() {#setdefaultstyle}

Gets or sets the default Style object of the workbook. The DefaultStyle property is useful to implement a Style for the whole Workbook.

### setDigitalSignature(digitalSignatureCollection) {#setdigitalsignature}

Sets digital signature to an spreadsheet file (Excel2007 and later). Only support adding Xmldsig Digital Signature

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### setEncryptionOptions(encryptionType, keyLength) {#setencryptionoptions}

Set Encryption Options.

| Parameter | Type | Description |
| --- | --- | --- |
| encryptionType | Number | EncryptionType |
| keyLength | Number | The key length. |

### setFileFormat() {#setfileformat}

Gets and sets the file format. The value of the property is FileFormatType integer constant.

### setFileName() {#setfilename}

Gets and sets the current file name. If the file is opened by stream and there are some external formula references, please set the file name.

### setInterruptMonitor() {#setinterruptmonitor}

Gets and sets the interrupt monitor.

### setRibbonXml() {#setribbonxml}

Gets and sets the XML file that defines the Ribbon UI.

### setThemeColor(type, color) {#setthemecolor}

Sets the theme color

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ThemeColorType |
| color | Color | the theme color |

### startAccessCache(opts) {#startaccesscache}

Starts the session that uses caches to access data. If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them. After finishing the access to the data, closeAccessCache(int) should be invoked with same options to clear all caches and recover normal access mode.

| Parameter | Type | Description |
| --- | --- | --- |
| opts | Number | AccessCacheOptions |

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

### updateCustomFunctionDefinition(definition) {#updatecustomfunctiondefinition}

Updates definition of custom functions. This method can be used for some special scenarios. For example, if user needs some parameters of some custom functions be calculated in array mode, then user may provide their own definition with implemented CustomFunctionDefinition.getArrayModeParameters(java.lang.String) for those functions. After the data of formulas being updated, those specified parameters will be calculated in array mode automatically when calculating corresponding custom functions.

| Parameter | Type | Description |
| --- | --- | --- |
| definition | CustomFunctionDefinition | Special definition of custom functions for user's special requirement. |

### updateLinkedDataSource(externalWorkbooks) {#updatelinkeddatasource}

If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources. If corresponding external link cannot be found for one workbook, then this workbook will be ignored. So when you set a formula later with one new external link which you intend to make the ignored workbook be linked to it, the link cannot be performed until you call this this method again with those workbooks.

| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | Array ofWorkbook | Workbooks that will be used to update data of external links referenced by this workbook. The match of those workbooks with external links is determined by |

### createWorkbookFromStream(stream, callback) (static) {#createworkbookfromstream}

Initializes a new instance of the Workbook class and open a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | ReadableStream | The stream |
| callback | Callback | The callback function |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var readStream = fs.createReadStream("Book2.xlsx");
aspose.cells.Workbook.createWorkbookFromStream(readStream, function(workbook, err) {
if (err) {
console.log("open workbook error");
return;
}
workbook.save('result.xlsx');
console.log('saved to file');
});
```

### createWorkbookFromStream(stream, loadOptions, callback) (static) {#createworkbookfromstream-1}

Initializes a new instance of the Workbook class and open a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | ReadableStream | The stream |
| loadOptions | LoadOptions | The load options |
| callback | Callback | The callback function |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var readStream = fs.createReadStream("Book2.xlsx");
var loadOptions = new aspose.cells.LoadOptions();
aspose.cells.Workbook.createWorkbookFromStream(readStream, loadOptions, function(workbook, err) {
if (err) {
console.log("open workbook error");
return;
}
workbook.save('result.xlsx');
console.log('saved to file');
});
```

### save(workbook, stream, saveOptions) (static) {#save-3}

Save the workbook to the stream.

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook object to save |
| stream | WritableStream | The stream |
| saveOptions | SaveOptions | The save options |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var saveOptions = new aspose.cells.XlsSaveOptions();
var writeStream = fs.createWriteStream("result-stream.xls");
aspose.cells.Workbook.saveToStream(workbook, writeStream, saveOptions);
```

### save(workbook, stream, saveFormat) (static) {#save-4}

Save the workbook to the stream.

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook object to save |
| stream | WritableStream | The stream |
| saveFormat | Number | The save file format type |

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var workbook = new aspose.cells.Workbook("Book2.xlsx");
var writeStream = fs.createWriteStream("result-stream.xlsx");
aspose.cells.Workbook.saveToStream(workbook, writeStream, aspose.cells.SaveFormat.XLSX);
```
