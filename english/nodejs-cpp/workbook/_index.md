﻿---
title: Workbook
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a root object to create an Excel spreadsheet.
type: docs
url: /nodejs-cpp/workbook/
---

## Workbook class

Represents a root object to create an Excel spreadsheet.

```javascript
class Workbook;
```

### Remarks
The Workbook class denotes an Excel spreadsheet. Each spreadsheet can contain multiple worksheets. The basic feature of the class is to open and save native excel files. The class has some advanced features like copying data from other Workbooks, combining two Workbooks, converting Excel to PDF, rendering Excel to image and protecting the Excel spreadsheet.

## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Initializes a new instance of the [Workbook](../workbook/) class. |
| [constructor(FileFormatType)](#constructor-fileformattype-)| Initializes a new instance of the [Workbook](../workbook/) class. |
| [constructor(string)](#constructor-string-)| Initializes a new instance of the [Workbook](../workbook/) class and open a file. |
| [constructor(Uint8Array)](#constructor-uint8array-)| Initializes a new instance of the [Workbook](../workbook/) class and open a stream. |
| [constructor(string, LoadOptions)](#constructor-string-loadoptions-)| Initializes a new instance of the [Workbook](../workbook/) class and open a file. |
| [constructor(Uint8Array, LoadOptions)](#constructor-uint8array-loadoptions-)| Initializes a new instance of the [Workbook](../workbook/) class and open stream. |

## Methods

| Method | Description |
| --- | --- |
| [getSettings()](#getSettings--)| Represents the workbook settings. |
| [getWorksheets()](#getWorksheets--)| Gets the [WorksheetCollection](../worksheetcollection/) collection in the spreadsheet. |
| [isLicensed()](#isLicensed--)| Indicates whether license is set. |
| [getColors()](#getColors--)| Returns colors in the palette for the spreadsheet. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--)| Gets number of the styles in the style pool. |
| [getDefaultStyle()](#getDefaultStyle--)| Gets or sets the default [Style](../style/) object of the workbook. |
| [setDefaultStyle(Style)](#setDefaultStyle-style-)| Gets or sets the default [Style](../style/) object of the workbook. |
| [isDigitallySigned()](#isDigitallySigned--)| Indicates if this spreadsheet is digitally signed. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--)| Indicates whether structure or window is protected with password. |
| [getVbaProject()](#getVbaProject--)| Gets the [VbaProject](../vbaproject/) in a spreadsheet. |
| [getHasMacro()](#getHasMacro--)| Indicates if this spreadsheet contains macro/VBA. |
| [getHasRevisions()](#getHasRevisions--)| Gets if the workbook has any tracked changes |
| [getFileName()](#getFileName--)| Gets and sets the current file name. |
| [setFileName(string)](#setFileName-string-)| Gets and sets the current file name. |
| [getDataSorter()](#getDataSorter--)| Gets a DataSorter object to sort data. |
| [getTheme()](#getTheme--)| Gets the theme name. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--)| Returns a [DocumentProperty](../documentproperty/) collection that represents all the built-in document properties of the spreadsheet. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--)| Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet. |
| [getFileFormat()](#getFileFormat--)| Gets and sets the file format. |
| [setFileFormat(FileFormatType)](#setFileFormat-fileformattype-)| Gets and sets the file format. |
| [getInterruptMonitor()](#getInterruptMonitor--)| Gets and sets the interrupt monitor. |
| [getContentTypeProperties()](#getContentTypeProperties--)| Gets the list of  [ContentTypeProperty](../contenttypeproperty/) objects in the workbook. |
| [getCustomXmlParts()](#getCustomXmlParts--)| Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [getDataMashup()](#getDataMashup--)| Gets mashup data. |
| [getRibbonXml()](#getRibbonXml--)| Gets and sets the XML file that defines the Ribbon UI. |
| [setRibbonXml(string)](#setRibbonXml-string-)| Gets and sets the XML file that defines the Ribbon UI. |
| [getAbsolutePath()](#getAbsolutePath--)| Gets and sets the absolute path of the file. |
| [setAbsolutePath(string)](#setAbsolutePath-string-)| Gets and sets the absolute path of the file. |
| [getDataConnections()](#getDataConnections--)| Gets the [ExternalConnection](../externalconnection/) collection. |
| [parseFormulas(boolean)](#parseFormulas-boolean-)| Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [startAccessCache(AccessCacheOptions)](#startAccessCache-accesscacheoptions-)| Starts the session that uses caches to access data. |
| [closeAccessCache(AccessCacheOptions)](#closeAccessCache-accesscacheoptions-)| Closes the session that uses caches to access data. |
| [save(string, SaveFormat)](#save-string-saveformat-)| Saves the workbook to the disk. |
| [save(string)](#save-string-)| Save the workbook to the disk. |
| [save(string, SaveOptions)](#save-string-saveoptions-)| Saves the workbook to the disk. |
| [save(SaveFormat)](#save-saveformat-)| Saves the workbook to the stream. |
| [save(SaveOptions)](#save-saveoptions-)| Saves the workbook to the stream. |
| [saveToStream()](#saveToStream--)| Saves Excel file to a MemoryStream object and returns it. |
| [removeUnusedStyles()](#removeUnusedStyles--)| Remove all unused styles. |
| [createStyle()](#createStyle--)| Creates a new style. |
| [createBuiltinStyle(BuiltinStyleType)](#createBuiltinStyle-builtinstyletype-)| Creates built-in style by given type. |
| [createCellsColor()](#createCellsColor--)| Creates a [CellsColor](../cellscolor/) object. |
| [replace(string, string)](#replace-string-string-)| Replaces a cell's value with a new string. |
| [replace(string, number)](#replace-string-number-)| Replaces a cell's value with a new integer. |
| [replace(string, number)](#replace-string-number-)| Replaces a cell's value with a new double. |
| [replace(string, string[], boolean)](#replace-string-stringarray-boolean-)| Replaces a cell's value with a new string array. |
| [replace(string, number[], boolean)](#replace-string-numberarray-boolean-)| Replaces cells' values with an integer array. |
| [replace(string, number[], boolean)](#replace-string-numberarray-boolean-)| Replaces cells' values with a double array. |
| [replace(boolean, object)](#replace-boolean-object-)| Replaces cells' values with new data. |
| [replace(number, object)](#replace-number-object-)| Replaces cells' values with new data. |
| [replace(string, string, ReplaceOptions)](#replace-string-string-replaceoptions-)| Replaces a cell's value with a new string. |
| [copy(Workbook, CopyOptions)](#copy-workbook-copyoptions-)| Copies another Workbook object. |
| [copy(Workbook)](#copy-workbook-)| Copies data from a source Workbook object. |
| [combine(Workbook)](#combine-workbook-)| Combines another Workbook object. |
| [getStyleInPool(number)](#getStyleInPool-number-)| Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells. |
| [getFonts()](#getFonts--)| Gets all fonts in the style pool. |
| [getNamedStyle(string)](#getNamedStyle-string-)| Gets the named style in the style pool. |
| [changePalette(Color, number)](#changePalette-color-number-)| Changes the palette for the spreadsheet in the specified index. |
| [isColorInPalette(Color)](#isColorInPalette-color-)| Checks if a color is in the palette for the spreadsheet. |
| [calculateFormula()](#calculateFormula--)| Calculates the result of formulas. |
| [calculateFormula(boolean)](#calculateFormula-boolean-)| Calculates the result of formulas. |
| [calculateFormula(CalculationOptions)](#calculateFormula-calculationoptions-)| Calculating formulas in this workbook. |
| [refreshDynamicArrayFormulas(boolean)](#refreshDynamicArrayFormulas-boolean-)| Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas. |
| [refreshDynamicArrayFormulas(boolean, CalculationOptions)](#refreshDynamicArrayFormulas-boolean-calculationoptions-)| Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) |
| [getMatchingColor(Color)](#getMatchingColor-color-)| Find best matching Color in current palette. |
| [setEncryptionOptions(EncryptionType, number)](#setEncryptionOptions-encryptiontype-number-)| Set Encryption Options. |
| [protect(ProtectionType, string)](#protect-protectiontype-string-)| Protects a workbook. |
| [protectSharedWorkbook(string)](#protectSharedWorkbook-string-)| Protects a shared workbook. |
| [unprotect(string)](#unprotect-string-)| Unprotects a workbook. |
| [unprotectSharedWorkbook(string)](#unprotectSharedWorkbook-string-)| Unprotects a shared workbook. |
| [removeMacro()](#removeMacro--)| Removes VBA/macro from this spreadsheet. |
| [removeDigitalSignature()](#removeDigitalSignature--)| Removes digital signature from this spreadsheet. |
| [acceptAllRevisions()](#acceptAllRevisions--)| Accepts all tracked changes in the workbook. |
| [getThemeColor(ThemeColorType)](#getThemeColor-themecolortype-)| Gets theme color. |
| [setThemeColor(ThemeColorType, Color)](#setThemeColor-themecolortype-color-)| Sets the theme color |
| [customTheme(string, Color[])](#customTheme-string-colorarray-)| Customs the theme. |
| [copyTheme(Workbook)](#copyTheme-workbook-)| Copies the theme from another workbook. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition)](#updateCustomFunctionDefinition-customfunctiondefinition-)| Updates definition of custom functions. |
| [updateLinkedDataSource(Workbook[])](#updateLinkedDataSource-workbookarray-)| If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources. |
| [setInterruptMonitor(InterruptMonitor)](#setInterruptMonitor-interruptmonitor-)| Sets the interrupt monitor. |
| [importXml(string, string, number, number)](#importXml-string-string-number-number-)| Imports/Updates an XML data file into the workbook. |
| [importXml(Uint8Array, string, number, number)](#importXml-uint8array-string-number-number-)| Imports/Updates an XML data file into the workbook. |
| [exportXml(string, string)](#exportXml-string-string-)| Export XML data linked by the specified XML map. |
| [exportXml(string)](#exportXml-string-)| Export XML data. |
| [setDigitalSignature(DigitalSignatureCollection)](#setDigitalSignature-digitalsignaturecollection-)| Sets digital signature to an spreadsheet file (Excel2007 and later). |
| [addDigitalSignature(DigitalSignatureCollection)](#addDigitalSignature-digitalsignaturecollection-)| Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). |
| [getDigitalSignature()](#getDigitalSignature--)| Gets digital signature from file. |
| [removePersonalInformation()](#removePersonalInformation--)| Removes personal information. |
| [dispose()](#dispose--)| Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Initializes a new instance of the [Workbook](../workbook/) class.

```javascript
constructor();
```


**Remarks**

The default file format type is Xlsx. If you want to create other types of files, please use Workbook(FileFormatType).

### constructor(FileFormatType) {#constructor-fileformattype-}

Initializes a new instance of the [Workbook](../workbook/) class.

```javascript
constructor(fileFormatType: FileFormatType);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileFormatType | [FileFormatType](../fileformattype/) | The new file format. |

**Remarks**

The default file format type is Excel97To2003.

### constructor(string) {#constructor-string-}

Initializes a new instance of the [Workbook](../workbook/) class and open a file.

```javascript
constructor(file: string);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | string | The file name. |

### constructor(Uint8Array) {#constructor-uint8array-}

Initializes a new instance of the [Workbook](../workbook/) class and open a stream.

```javascript
constructor(stream: Uint8Array);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | The stream. |

### constructor(string, LoadOptions) {#constructor-string-loadoptions-}

Initializes a new instance of the [Workbook](../workbook/) class and open a file.

```javascript
constructor(file: string, loadOptions: LoadOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | string | The file name. |
| loadOptions | [LoadOptions](../loadoptions/) | The load options |

### constructor(Uint8Array, LoadOptions) {#constructor-uint8array-loadoptions-}

Initializes a new instance of the [Workbook](../workbook/) class and open stream.

```javascript
constructor(stream: Uint8Array, loadOptions: LoadOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | The stream. |
| loadOptions | [LoadOptions](../loadoptions/) | The load options |

### getSettings() {#getSettings--}

Represents the workbook settings.

```javascript
getSettings() : WorkbookSettings;
```


**Returns**

[WorkbookSettings](../workbooksettings/)

### getWorksheets() {#getWorksheets--}

Gets the [WorksheetCollection](../worksheetcollection/) collection in the spreadsheet.

```javascript
getWorksheets() : WorksheetCollection;
```


**Returns**

[WorksheetCollection](../worksheetcollection/) collection

### isLicensed() {#isLicensed--}

Indicates whether license is set.

```javascript
isLicensed() : boolean;
```


### getColors() {#getColors--}

Returns colors in the palette for the spreadsheet.

```javascript
getColors() : Color[];
```


**Returns**

[Color](../color/)[]

**Remarks**

The palette has 56 entries, each represented by an RGB value.

### getCountOfStylesInPool() {#getCountOfStylesInPool--}

Gets number of the styles in the style pool.

```javascript
getCountOfStylesInPool() : number;
```


### getDefaultStyle() {#getDefaultStyle--}

Gets or sets the default [Style](../style/) object of the workbook.

```javascript
getDefaultStyle() : Style;
```


**Returns**

[Style](../style/)

**Remarks**

The DefaultStyle property is useful to implement a Style for the whole Workbook.

### setDefaultStyle(Style) {#setDefaultStyle-style-}

Gets or sets the default [Style](../style/) object of the workbook.

```javascript
setDefaultStyle(value: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../style/) | The value to set. |

**Remarks**

The DefaultStyle property is useful to implement a Style for the whole Workbook.

### isDigitallySigned() {#isDigitallySigned--}

Indicates if this spreadsheet is digitally signed.

```javascript
isDigitallySigned() : boolean;
```


### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}

Indicates whether structure or window is protected with password.

```javascript
isWorkbookProtectedWithPassword() : boolean;
```


### getVbaProject() {#getVbaProject--}

Gets the [VbaProject](../vbaproject/) in a spreadsheet.

```javascript
getVbaProject() : VbaProject;
```


**Returns**

[VbaProject](../vbaproject/)

### getHasMacro() {#getHasMacro--}

Indicates if this spreadsheet contains macro/VBA.

```javascript
getHasMacro() : boolean;
```


### getHasRevisions() {#getHasRevisions--}

Gets if the workbook has any tracked changes

```javascript
getHasRevisions() : boolean;
```


### getFileName() {#getFileName--}

Gets and sets the current file name.

```javascript
getFileName() : string;
```


**Remarks**

If the file is opened by stream and there are some external formula references, please set the file name.

### setFileName(string) {#setFileName-string-}

Gets and sets the current file name.

```javascript
setFileName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If the file is opened by stream and there are some external formula references, please set the file name.

### getDataSorter() {#getDataSorter--}

Gets a DataSorter object to sort data.

```javascript
getDataSorter() : DataSorter;
```


**Returns**

[DataSorter](../datasorter/)

### getTheme() {#getTheme--}

Gets the theme name.

```javascript
getTheme() : string;
```


### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}

Returns a [DocumentProperty](../documentproperty/) collection that represents all the built-in document properties of the spreadsheet.

```javascript
getBuiltInDocumentProperties() : BuiltInDocumentPropertyCollection;
```


**Returns**

[BuiltInDocumentPropertyCollection](../builtindocumentpropertycollection/)

**Remarks**

A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list: <p>Title</p> <p>Subject</p> <p>Author</p> <p>Keywords</p> <p>Comments</p> <p>Template</p> <p>Last Author</p> <p>Revision Number</p> <p>Application Name</p> <p>Last Print Date</p> <p>Creation Date</p> <p>Last Save Time</p> <p>Total Editing Time</p> <p>Number of Pages</p> <p>Number of Words</p> <p>Number of Characters</p> <p>Security</p> <p>Category</p> <p>Format</p> <p>Manager</p> <p>Company</p> <p>Number of Bytes</p> <p>Number of Lines</p> <p>Number of Paragraphs</p> <p>Number of Slides</p> <p>Number of Notes</p> <p>Number of Hidden Slides</p> <p>Number of Multimedia Clips</p>

### getCustomDocumentProperties() {#getCustomDocumentProperties--}

Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet.

```javascript
getCustomDocumentProperties() : CustomDocumentPropertyCollection;
```


**Returns**

[CustomDocumentPropertyCollection](../customdocumentpropertycollection/)

### getFileFormat() {#getFileFormat--}

Gets and sets the file format.

```javascript
getFileFormat() : FileFormatType;
```


**Returns**

[FileFormatType](../fileformattype/)

### setFileFormat(FileFormatType) {#setFileFormat-fileformattype-}

Gets and sets the file format.

```javascript
setFileFormat(value: FileFormatType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FileFormatType](../fileformattype/) | The value to set. |

### getInterruptMonitor() {#getInterruptMonitor--}

Gets and sets the interrupt monitor.

```javascript
getInterruptMonitor() : AbstractInterruptMonitor;
```


**Returns**

[AbstractInterruptMonitor](../abstractinterruptmonitor/)

### getContentTypeProperties() {#getContentTypeProperties--}

Gets the list of  [ContentTypeProperty](../contenttypeproperty/) objects in the workbook.

```javascript
getContentTypeProperties() : ContentTypePropertyCollection;
```


**Returns**

[ContentTypePropertyCollection](../contenttypepropertycollection/)

### getCustomXmlParts() {#getCustomXmlParts--}

Represents a Custom XML Data Storage Part (custom XML data within a package).

```javascript
getCustomXmlParts() : CustomXmlPartCollection;
```


**Returns**

[CustomXmlPartCollection](../customxmlpartcollection/)

### getDataMashup() {#getDataMashup--}

Gets mashup data.

```javascript
getDataMashup() : DataMashup;
```


**Returns**

[DataMashup](../datamashup/)

### getRibbonXml() {#getRibbonXml--}

Gets and sets the XML file that defines the Ribbon UI.

```javascript
getRibbonXml() : string;
```


### setRibbonXml(string) {#setRibbonXml-string-}

Gets and sets the XML file that defines the Ribbon UI.

```javascript
setRibbonXml(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAbsolutePath() {#getAbsolutePath--}

Gets and sets the absolute path of the file.

```javascript
getAbsolutePath() : string;
```


**Remarks**

Only used for external links.

### setAbsolutePath(string) {#setAbsolutePath-string-}

Gets and sets the absolute path of the file.

```javascript
setAbsolutePath(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

Only used for external links.

### getDataConnections() {#getDataConnections--}

Gets the [ExternalConnection](../externalconnection/) collection.

```javascript
getDataConnections() : ExternalConnectionCollection;
```


**Returns**

[ExternalConnectionCollection](../externalconnectioncollection/)

### parseFormulas(boolean) {#parseFormulas-boolean-}

Parses all formulas which have not been parsed when they were loaded from template file or set to a cell.

```javascript
parseFormulas(ignoreError: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Whether ignore error for invalid formula.         /// For one invalid formula, if ignore error then this formula will be ignored         /// and the process will continue to parse other formulas, otherwise exception will be thrown. |

### startAccessCache(AccessCacheOptions) {#startAccessCache-accesscacheoptions-}

Starts the session that uses caches to access data.

```javascript
startAccessCache(opts: AccessCacheOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | [AccessCacheOptions](../accesscacheoptions/) | options of data access |

**Remarks**

If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them. <br></br> After finishing the access to the data, [CloseAccessCache(AccessCacheOptions)](../closeaccesscache(accesscacheoptions)/) should be invoked with same options to clear all caches and recover normal access mode. <br></br>

### closeAccessCache(AccessCacheOptions) {#closeAccessCache-accesscacheoptions-}

Closes the session that uses caches to access data.

```javascript
closeAccessCache(opts: AccessCacheOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | [AccessCacheOptions](../accesscacheoptions/) | options of data access |

### save(string, SaveFormat) {#save-string-saveformat-}

Saves the workbook to the disk.

```javascript
save(fileName: string, saveFormat: SaveFormat) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The file name. |
| saveFormat | [SaveFormat](../saveformat/) | The save format type. |

### save(string) {#save-string-}

Save the workbook to the disk.

```javascript
save(fileName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string |  |

### save(string, SaveOptions) {#save-string-saveoptions-}

Saves the workbook to the disk.

```javascript
save(fileName: string, saveOptions: SaveOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The file name. |
| saveOptions | [SaveOptions](../saveoptions/) | The save options. |

### save(SaveFormat) {#save-saveformat-}

Saves the workbook to the stream.

```javascript
save(saveFormat: SaveFormat) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](../saveformat/) | The save file format type. |

**Returns**

The result stream

### save(SaveOptions) {#save-saveoptions-}

Saves the workbook to the stream.

```javascript
save(saveOptions: SaveOptions) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../saveoptions/) | The save options. |

**Returns**

The result stream

### saveToStream() {#saveToStream--}

Saves Excel file to a MemoryStream object and returns it.

```javascript
saveToStream() : Uint8Array;
```


**Returns**

MemoryStream object which contains an Excel file.

**Remarks**

This method provides same function as Save method and only save the workbook as Excel97-2003 xls file. It's mainly for calling from COM clients.

### removeUnusedStyles() {#removeUnusedStyles--}

Remove all unused styles.

```javascript
removeUnusedStyles() : void;
```


### createStyle() {#createStyle--}

Creates a new style.

```javascript
createStyle() : Style;
```


**Returns**

Returns a style object.

### createBuiltinStyle(BuiltinStyleType) {#createBuiltinStyle-builtinstyletype-}

Creates built-in style by given type.

```javascript
createBuiltinStyle(type: BuiltinStyleType) : Style;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [BuiltinStyleType](../builtinstyletype/) | The builtin style stype. |

**Returns**

[Style](../style/) object

### createCellsColor() {#createCellsColor--}

Creates a [CellsColor](../cellscolor/) object.

```javascript
createCellsColor() : CellsColor;
```


**Returns**

Returns a [CellsColor](../cellscolor/) object.

### replace(string, string) {#replace-string-string-}

Replaces a cell's value with a new string.

```javascript
replace(placeHolder: string, newValue: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | string | Cell placeholder |
| newValue | string | String value to replace |

### replace(string, number) {#replace-string-number-}

Replaces a cell's value with a new integer.

```javascript
replace(placeHolder: string, newValue: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | string | Cell placeholder |
| newValue | number | Integer value to replace |

### replace(string, number) {#replace-string-number-}

Replaces a cell's value with a new double.

```javascript
replace(placeHolder: string, newValue: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | string | Cell placeholder |
| newValue | number | Double value to replace |

### replace(string, string[], boolean) {#replace-string-stringarray-boolean-}

Replaces a cell's value with a new string array.

```javascript
replace(placeHolder: string, newValues: string[], isVertical: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | string | Cell placeholder |
| newValues | string[] | String array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

### replace(string, number[], boolean) {#replace-string-numberarray-boolean-}

Replaces cells' values with an integer array.

```javascript
replace(placeHolder: string, newValues: number[], isVertical: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | string | Cell placeholder |
| newValues | number[] | Integer array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

### replace(string, number[], boolean) {#replace-string-numberarray-boolean-}

Replaces cells' values with a double array.

```javascript
replace(placeHolder: string, newValues: number[], isVertical: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | string | Cell placeholder |
| newValues | number[] | Double array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

### replace(boolean, object) {#replace-boolean-object-}

Replaces cells' values with new data.

```javascript
replace(boolValue: boolean, newValue: object) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | boolean | The boolean value to be replaced. |
| newValue | object | New value. Can be string, integer, double or DateTime value. |

### replace(number, object) {#replace-number-object-}

Replaces cells' values with new data.

```javascript
replace(intValue: number, newValue: object) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| intValue | number | The integer value to be replaced. |
| newValue | object | New value. Can be string, integer, double or DateTime value. |

### replace(string, string, ReplaceOptions) {#replace-string-string-replaceoptions-}

Replaces a cell's value with a new string.

```javascript
replace(placeHolder: string, newValue: string, options: ReplaceOptions) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | string | Cell placeholder |
| newValue | string | String value to replace |
| options | [ReplaceOptions](../replaceoptions/) | The replace options |

### copy(Workbook, CopyOptions) {#copy-workbook-copyoptions-}

Copies another Workbook object.

```javascript
copy(source: Workbook, copyOptions: CopyOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Workbook](../workbook/) | Source Workbook object. |
| copyOptions | [CopyOptions](../copyoptions/) | The options of copying other workbook. |

**Remarks**

It's very simple to clone an Excel file.

### copy(Workbook) {#copy-workbook-}

Copies data from a source Workbook object.

```javascript
copy(source: Workbook) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Workbook](../workbook/) | Source Workbook object. |

### combine(Workbook) {#combine-workbook-}

Combines another Workbook object.

```javascript
combine(secondWorkbook: Workbook) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| secondWorkbook | [Workbook](../workbook/) | Another Workbook object. |

**Remarks**

Merge Excel, ODS , CSV and other files to one file.

### getStyleInPool(number) {#getStyleInPool-number-}

Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells.

```javascript
getStyleInPool(index: number) : Style;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

The style in the pool corresponds to given index, may be null.

**Remarks**

If the returned style is changed, the style of all cells(which refers to this style) will be changed.

### getFonts() {#getFonts--}

Gets all fonts in the style pool.

```javascript
getFonts() : Font[];
```


**Returns**

[Font](../font/)[]

### getNamedStyle(string) {#getNamedStyle-string-}

Gets the named style in the style pool.

```javascript
getNamedStyle(name: string) : Style;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | name of the style |

**Returns**

named style, maybe null.

### changePalette(Color, number) {#changePalette-color-number-}

Changes the palette for the spreadsheet in the specified index.

```javascript
changePalette(color: Color, index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../color/) | Color structure. |
| index | number | Palette index, 0 - 55. |

**Remarks**

<p>The palette has 56 entries, each represented by an RGB value.</p> <p>If you set a color which is not in the palette, it will not take effect.</p> <p>So if you want to set a custom color, please change the palette at first.</p> <p>The following is the standard color palette.</p> <list type="table"> <listheader> <description>Color</description> <description>Red</description> <description>Green</description> <description>Blue</description> </listheader> <item> <description>Black</description> <description>0</description> <description>0</description> <description>0</description> </item> <item> <description>White</description> <description>255</description> <description>255</description> <description>255</description> </item> <item> <description>Red</description> <description>255</description> <description>0</description> <description>0</description> </item> <item> <description>Lime</description> <description>0</description> <description>255</description> <description>0</description> </item> <item> <description>Blue</description> <description>0</description> <description>0</description> <description>255</description> </item> <item> <description>Yellow</description> <description>255</description> <description>255</description> <description>0</description> </item> <item> <description>Magenta</description> <description>255</description> <description>0</description> <description>255</description> </item> <item> <description>Cyan</description> <description>0</description> <description>255</description> <description>255</description> </item> <item> <description>Maroon</description> <description>128</description> <description>0</description> <description>0</description> </item> <item> <description>Green</description> <description>0</description> <description>128</description> <description>0</description> </item> <item> <description>Navy</description> <description>0</description> <description>0</description> <description>128</description> </item> <item> <description>Olive</description> <description>128</description> <description>128</description> <description>0</description> </item> <item> <description>Purple</description> <description>128</description> <description>0</description> <description>128</description> </item> <item> <description>Teal</description> <description>0</description> <description>128</description> <description>128</description> </item> <item> <description>Silver</description> <description>192</description> <description>192</description> <description>192</description> </item> <item> <description>Gray</description> <description>128</description> <description>128</description> <description>128</description> </item> <item> <description>Color17</description> <description>153</description> <description>153</description> <description>255</description> </item> <item> <description>Color18</description> <description>153</description> <description>51</description> <description>102</description> </item> <item> <description>Color19</description> <description>255</description> <description>255</description> <description>204</description> </item> <item> <description>Color20</description> <description>204</description> <description>255</description> <description>255</description> </item> <item> <description>Color21</description> <description>102</description> <description>0</description> <description>102</description> </item> <item> <description>Color22</description> <description>255</description> <description>128</description> <description>128</description> </item> <item> <description>Color23</description> <description>0</description> <description>102</description> <description>204</description> </item> <item> <description>Color24</description> <description>204</description> <description>204</description> <description>255</description> </item> <item> <description>Color25</description> <description>0</description> <description>0</description> <description>128</description> </item> <item> <description>Color26</description> <description>255</description> <description>0</description> <description>255</description> </item> <item> <description>Color27</description> <description>255</description> <description>255</description> <description>0</description> </item> <item> <description>Color28</description> <description>0</description> <description>255</description> <description>255</description> </item> <item> <description>Color29</description> <description>128</description> <description>0</description> <description>128</description> </item> <item> <description>Color30</description> <description>128</description> <description>0</description> <description>0</description> </item> <item> <description>Color31</description> <description>0</description> <description>128</description> <description>128</description> </item> <item> <description>Color32</description> <description>0</description> <description>0</description> <description>255</description> </item> <item> <description>Color33</description> <description>0</description> <description>204</description> <description>255</description> </item> <item> <description>Color34</description> <description>204</description> <description>255</description> <description>255</description> </item> <item> <description>Color35</description> <description>204</description> <description>255</description> <description>204</description> </item> <item> <description>Color36</description> <description>255</description> <description>255</description> <description>153</description> </item> <item> <description>Color37</description> <description>153</description> <description>204</description> <description>255</description> </item> <item> <description>Color38</description> <description>255</description> <description>153</description> <description>204</description> </item> <item> <description>Color39</description> <description>204</description> <description>153</description> <description>255</description> </item> <item> <description>Color40</description> <description>255</description> <description>204</description> <description>153</description> </item> <item> <description>Color41</description> <description>51</description> <description>102</description> <description>255</description> </item> <item> <description>Color42</description> <description>51</description> <description>204</description> <description>204</description> </item> <item> <description>Color43</description> <description>153</description> <description>204</description> <description>0</description> </item> <item> <description>Color44</description> <description>255</description> <description>204</description> <description>0</description> </item> <item> <description>Color45</description> <description>255</description> <description>153</description> <description>0</description> </item> <item> <description>Color46</description> <description>255</description> <description>102</description> <description>0</description> </item> <item> <description>Color47</description> <description>102</description> <description>102</description> <description>153</description> </item> <item> <description>Color48</description> <description>150</description> <description>150</description> <description>150</description> </item> <item> <description>Color49</description> <description>0</description> <description>51</description> <description>102</description> </item> <item> <description>Color50</description> <description>51</description> <description>153</description> <description>102</description> </item> <item> <description>Color51</description> <description>0</description> <description>51</description> <description>0</description> </item> <item> <description>Color52</description> <description>51</description> <description>51</description> <description>0</description> </item> <item> <description>Color53</description> <description>153</description> <description>51</description> <description>0</description> </item> <item> <description>Color54</description> <description>153</description> <description>51</description> <description>102</description> </item> <item> <description>Color55</description> <description>51</description> <description>51</description> <description>153</description> </item> <item> <description>Color56</description> <description>51</description> <description>51</description> <description>51</description> </item> </list>

### isColorInPalette(Color) {#isColorInPalette-color-}

Checks if a color is in the palette for the spreadsheet.

```javascript
isColorInPalette(color: Color) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../color/) | Color structure. |

**Returns**

Returns true if this color is in the palette. Otherwise, returns false

### calculateFormula() {#calculateFormula--}

Calculates the result of formulas.

```javascript
calculateFormula() : void;
```


**Remarks**

For all supported formulas, please see the list at https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean) {#calculateFormula-boolean-}

Calculates the result of formulas.

```javascript
calculateFormula(ignoreError: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |

### calculateFormula(CalculationOptions) {#calculateFormula-calculationoptions-}

Calculating formulas in this workbook.

```javascript
calculateFormula(options: CalculationOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../calculationoptions/) | Options for calculation |

### refreshDynamicArrayFormulas(boolean) {#refreshDynamicArrayFormulas-boolean-}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.

```javascript
refreshDynamicArrayFormulas(calculate: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |

### refreshDynamicArrayFormulas(boolean, CalculationOptions) {#refreshDynamicArrayFormulas-boolean-calculationoptions-}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)

```javascript
refreshDynamicArrayFormulas(calculate: boolean, copts: CalculationOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |
| copts | [CalculationOptions](../calculationoptions/) | The options for calculating formulas |

**Remarks**

For performance consideration, we do not refresh all dynamic array formulas automatically when the formula itself or the data it references to changed. So user need to call this method manually after those operations which may influence dynamic array formulas, such as importing/setting cell values, inserting/deleting rows/columns/ranges, ...etc.<br></br> For most formulas with functions, calculating the spill range also needs to calculating the formula, so in general true value for "calculate" flag is preferred. If the formula is simple, such as a range reference or array(for example "=C1:E5", "={1,2;3,4}", ...), simple function on a range or array(for example "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), and all formulas will be calculated later(such as by [Workbook.CalculateFormula(CalculationOptions)](../workbook.calculateformula(calculationoptions)/)), then using false vlaue for "calculate" flag may avoid the duplicated calculation for the benefit of performance.

### getMatchingColor(Color) {#getMatchingColor-color-}

Find best matching Color in current palette.

```javascript
getMatchingColor(rawColor: Color) : Color;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rawColor | [Color](../color/) | Raw color. |

**Returns**

Best matching color.

### setEncryptionOptions(EncryptionType, number) {#setEncryptionOptions-encryptiontype-number-}

Set Encryption Options.

```javascript
setEncryptionOptions(encryptionType: EncryptionType, keyLength: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| encryptionType | [EncryptionType](../encryptiontype/) | The encryption type. |
| keyLength | number | The key length. |

### protect(ProtectionType, string) {#protect-protectiontype-string-}

Protects a workbook.

```javascript
protect(protectionType: ProtectionType, password: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| protectionType | [ProtectionType](../protectiontype/) | Protection type. |
| password | string | Password to protect the workbook. |

### protectSharedWorkbook(string) {#protectSharedWorkbook-string-}

Protects a shared workbook.

```javascript
protectSharedWorkbook(password: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | Password to protect the workbook. |

### unprotect(string) {#unprotect-string-}

Unprotects a workbook.

```javascript
unprotect(password: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | Password to unprotect the workbook. |

### unprotectSharedWorkbook(string) {#unprotectSharedWorkbook-string-}

Unprotects a shared workbook.

```javascript
unprotectSharedWorkbook(password: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | Password to unprotect the workbook. |

### removeMacro() {#removeMacro--}

Removes VBA/macro from this spreadsheet.

```javascript
removeMacro() : void;
```


### removeDigitalSignature() {#removeDigitalSignature--}

Removes digital signature from this spreadsheet.

```javascript
removeDigitalSignature() : void;
```


### acceptAllRevisions() {#acceptAllRevisions--}

Accepts all tracked changes in the workbook.

```javascript
acceptAllRevisions() : void;
```


### getThemeColor(ThemeColorType) {#getThemeColor-themecolortype-}

Gets theme color.

```javascript
getThemeColor(type: ThemeColorType) : Color;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ThemeColorType](../themecolortype/) | The theme color type. |

**Returns**

The theme color.

### setThemeColor(ThemeColorType, Color) {#setThemeColor-themecolortype-color-}

Sets the theme color

```javascript
setThemeColor(type: ThemeColorType, color: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ThemeColorType](../themecolortype/) | The theme color type. |
| color | [Color](../color/) | the theme color |

### customTheme(string, Color[]) {#customTheme-string-colorarray-}

Customs the theme.

```javascript
customTheme(themeName: string, colors: Color[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| themeName | string | The theme name |
| colors | [Color](../color/)[] | The theme colors |

**Remarks**

The length of colors should be 12. <list type="table"> <listheader> <description>Array index</description> <description>Theme type</description> </listheader> <item> <description>0</description> <description>Backgournd1</description> </item> <item> <description>1</description> <description>Text1</description> </item> <item> <description>2</description> <description>Backgournd2</description> </item> <item> <description>3</description> <description>Text2</description> </item> <item> <description>4</description> <description>Accent1</description> </item> <item> <description>5</description> <description>Accent2</description> </item> <item> <description>6</description> <description>Accent3</description> </item> <item> <description>7</description> <description>Accent4</description> </item> <item> <description>8</description> <description>Accent5</description> </item> <item> <description>9</description> <description>Accent6</description> </item> <item> <description>10</description> <description>Hyperlink</description> </item> <item> <description>11</description> <description>Followed Hyperlink</description> </item> </list>

### copyTheme(Workbook) {#copyTheme-workbook-}

Copies the theme from another workbook.

```javascript
copyTheme(source: Workbook) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Workbook](../workbook/) | Source workbook. |

### updateCustomFunctionDefinition(CustomFunctionDefinition) {#updateCustomFunctionDefinition-customfunctiondefinition-}

Updates definition of custom functions.

```javascript
updateCustomFunctionDefinition(definition: CustomFunctionDefinition) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../customfunctiondefinition/) | Special definition of custom functions for user's special requirement. |

**Remarks**

This method can be used for some special scenarios. For example, if user needs some parameters of some custom functions be calculated in array mode, then user may provide their own definition with implemented [CustomFunctionDefinition.GetArrayModeParameters(string)](../customfunctiondefinition.getarraymodeparameters(string)/) for those functions. After the data of formulas being updated, those specified parameters will be calculated in array mode automatically when calculating corresponding custom functions.

### updateLinkedDataSource(Workbook[]) {#updateLinkedDataSource-workbookarray-}

If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources.

```javascript
updateLinkedDataSource(externalWorkbooks: Workbook[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | [Workbook](../workbook/)[] | Workbooks that will be used to update data of external links referenced by this workbook.         /// The match of those workbooks with external links is determined by [Workbook.FileName](../workbook.filename/)         /// and [Workbook.FileName](../workbook.filename/). So please make sure [Workbook.FileName](../workbook.filename/) has         /// been specified with the proper value for every workbook so they can be linked to corresponding external link. |

**Remarks**

If corresponding external link cannot be found for one workbook, then this workbook will be ignored. So when you set a formula later with one new external link which you intend to make the ignored workbook be linked to it, the link cannot be performed until you call this this method again with those workbooks.

### setInterruptMonitor(InterruptMonitor) {#setInterruptMonitor-interruptmonitor-}

Sets the interrupt monitor.

```javascript
setInterruptMonitor(interruptMonitor: InterruptMonitor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| interruptMonitor | [InterruptMonitor](../interruptmonitor/) | An InterruptMonitor object. |

### importXml(string, string, number, number) {#importXml-string-string-number-number-}

Imports/Updates an XML data file into the workbook.

```javascript
importXml(url: string, sheetName: string, row: number, col: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| url | string | the url/path of the xml file. |
| sheetName | string | the destination sheet name. |
| row | number | the destination row |
| col | number | the destination column |

### importXml(Uint8Array, string, number, number) {#importXml-uint8array-string-number-number-}

Imports/Updates an XML data file into the workbook.

```javascript
importXml(stream: Uint8Array, sheetName: string, row: number, col: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | the xml file stream. |
| sheetName | string | the destination sheet name. |
| row | number | the destination row. |
| col | number | the destination column. |

### exportXml(string, string) {#exportXml-string-string-}

Export XML data linked by the specified XML map.

```javascript
exportXml(mapName: string, path: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | string | name of the XML map that need to be exported |
| path | string | the export path |

### exportXml(string) {#exportXml-string-}

Export XML data.

```javascript
exportXml(mapName: string) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | string | name of the XML map that need to be exported |

**Returns**

The result stream

### setDigitalSignature(DigitalSignatureCollection) {#setDigitalSignature-digitalsignaturecollection-}

Sets digital signature to an spreadsheet file (Excel2007 and later).

```javascript
setDigitalSignature(digitalSignatureCollection: DigitalSignatureCollection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../digitalsignaturecollection/) |  |

**Remarks**

Only support adding Xmldsig Digital Signature

### addDigitalSignature(DigitalSignatureCollection) {#addDigitalSignature-digitalsignaturecollection-}

Adds digital signature to an OOXML spreadsheet file (Excel2007 and later).

```javascript
addDigitalSignature(digitalSignatureCollection: DigitalSignatureCollection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../digitalsignaturecollection/) |  |

**Remarks**

Only support adding Xmldsig Digital Signature to an OOXML spreadsheet file

### getDigitalSignature() {#getDigitalSignature--}

Gets digital signature from file.

```javascript
getDigitalSignature() : DigitalSignatureCollection;
```


**Returns**

[DigitalSignatureCollection](../digitalsignaturecollection/)

### removePersonalInformation() {#removePersonalInformation--}

Removes personal information.

```javascript
removePersonalInformation() : void;
```


### dispose() {#dispose--}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

```javascript
dispose() : void;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



