---
title: Workbook
second_title: Aspose.Cells for Java API Reference
description: Represents a root object to create an Excel spreadsheet.
type: docs
url: /java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

Represents a root object to create an Excel spreadsheet. The Workbook class denotes an Excel spreadsheet. Each spreadsheet can contain multiple worksheets. The basic feature of the class is to open and save native excel files. The class has some advanced features like copying data from other Workbooks, combining two Workbooks and protecting the Excel spreadsheet.

```
//Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xls");
```
## Constructors

| Constructor | Description |
| --- | --- |
| [Workbook()](#Workbook--) | Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class. |
| [Workbook(int fileFormatType)](#Workbook-int-) | Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class. |
| [Workbook(String file)](#Workbook-java.lang.String-) | Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class and open a file. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class and open a stream. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class and open a file. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class and open stream. |
## Methods

| Method | Description |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | Accepts all tracked changes in the workbook. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). |
| [calculateFormula()](#calculateFormula--) | Calculates the result of formulas. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | Calculates the result of formulas. |
| [calculateFormula(boolean ignoreError, ICustomFunction customFunction)](#calculateFormula-boolean-com.aspose.cells.ICustomFunction-) | Calculates the result of formulas. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | Calculating formulas in this workbook. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | Changes the palette for the spreadsheet in the specified index. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Closes the session that uses caches to access data. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | Combines another Workbook object. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | Copies data from a source Workbook object. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | Copies data from a source Workbook object. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | Copies the theme from another workbook. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | Creates built-in style by given type. |
| [createCellsColor()](#createCellsColor--) | Creates a [CellsColor](../../com.aspose.cells/cellscolor) object. |
| [createStyle()](#createStyle--) | Creates a new style. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | Customs the theme. |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | Export XML data linked by the specified XML map. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | Export XML data linked by the specified XML map. |
| [getAbsolutePath()](#getAbsolutePath--) | the absolute path of the file. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) collection that represents all the built-in document properties of the spreadsheet. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | Gets the factory for building ICellsDataTable from custom objects |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | Returns colors in the palette for the spreadsheet. |
| [getContentTypeProperties()](#getContentTypeProperties--) | Gets the list of [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) objects in the workbook. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | Gets number of the styles in the style pool. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) collection that represents all the custom document properties of the spreadsheet. |
| [getCustomXmlParts()](#getCustomXmlParts--) | Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [getDataConnections()](#getDataConnections--) | Gets the [ExternalConnection](../../com.aspose.cells/externalconnection) collection. |
| [getDataMashup()](#getDataMashup--) | Gets mashup data. |
| [getDataSorter()](#getDataSorter--) | Gets a DataSorter object to sort data. |
| [getDefaultStyle()](#getDefaultStyle--) | the default [Style](../../com.aspose.cells/style) object of the workbook. |
| [getDigitalSignature()](#getDigitalSignature--) | Gets digital signature from file. |
| [getFileFormat()](#getFileFormat--) | the file format. |
| [getFileName()](#getFileName--) | the current file name. |
| [getFonts()](#getFonts--) | Gets all fonts in the style pool. |
| [getInterruptMonitor()](#getInterruptMonitor--) | the interrupt monitor. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | Find best matching Color in current palette. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | Gets the named style in the style pool. |
| [getRibbonXml()](#getRibbonXml--) | the XML file that defines the Ribbon UI. |
| [getSettings()](#getSettings--) | Represents the workbook settings. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | Gets the style in the style pool. |
| [getTheme()](#getTheme--) | Gets the theme name. |
| [getThemeColor(int type)](#getThemeColor-int-) | Gets theme color. |
| [getVbaProject()](#getVbaProject--) | Gets the [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) in a spreadsheet. |
| [getWorksheets()](#getWorksheets--) | Gets the [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection in the spreadsheet. |
| [hasExernalLinks()](#hasExernalLinks--) | Indicates whether this workbook contains external links to other data sources. |
| [hasMacro()](#hasMacro--) | Indicates if this spreadsheet contains macro/VBA. |
| [hasRevisions()](#hasRevisions--) | Gets if the workbook has any tracked changes |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | Imports/Updates an XML data file into the workbook. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | Imports/Updates an XML data file into the workbook. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | Checks if a color is in the palette for the spreadsheet. |
| [isDigitallySigned()](#isDigitallySigned--) | Indicates if this spreadsheet is digitally signed. |
| [isLicensed()](#isLicensed--) | Indicates whether license is set. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | Indicates whether structure or window is protected with password. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | Protects a workbook. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | Protects a shared workbook. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) |
| [removeDigitalSignature()](#removeDigitalSignature--) | Removes digital signature from this spreadsheet. |
| [removeExternalLinks()](#removeExternalLinks--) | Removes all external links in the workbook. |
| [removeMacro()](#removeMacro--) | Removes VBA/macro from this spreadsheet. |
| [removePersonalInformation()](#removePersonalInformation--) | Removes personal information. |
| [removeUnusedStyles()](#removeUnusedStyles--) | Remove all unused styles. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | Replaces cells' values with new data. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | Replaces cells' values with new data. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | Replaces a cell's value with a new double. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | Replaces cells' values with a double array. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | Replaces a cell's value with a new integer. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | Replaces cells' values with an integer array. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | Replaces a cell's value with a new string. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Replaces a cell's value with a new string. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | Replaces a cell's value with a new string array. |
| [save(InputStream stream, SaveOptions saveOptions)](#save-java.io.InputStream-com.aspose.cells.SaveOptions-) | Saves the workbook to the stream. |
| [save(InputStream stream, int saveFormat)](#save-java.io.InputStream-int-) | Saves the workbook to the stream. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | Save the workbook to the stream. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | Save the workbook to the stream. |
| [save(String fileName)](#save-java.lang.String-) | Save the workbook to the disk. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | Saves the workbook to the disk. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | Saves the workbook to the disk. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | For the description of this property, please see [getAbsolutePath()](../../com.aspose.cells/workbook\#getAbsolutePath--) |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | For the description of this property, please see [getDefaultStyle()](../../com.aspose.cells/workbook\#getDefaultStyle--) |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Sets digital signature to an spreadsheet file (Excel2007 and later). |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | Set Encryption Options. |
| [setFileFormat(int value)](#setFileFormat-int-) | For the description of this property, please see [getFileFormat()](../../com.aspose.cells/workbook\#getFileFormat--) |
| [setFileName(String value)](#setFileName-java.lang.String-) | For the description of this property, please see [getFileName()](../../com.aspose.cells/workbook\#getFileName--) |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | For the description of this property, please see [getInterruptMonitor()](../../com.aspose.cells/workbook\#getInterruptMonitor--) |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | For the description of this property, please see [getRibbonXml()](../../com.aspose.cells/workbook\#getRibbonXml--) |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | Sets the theme color |
| [startAccessCache(int opts)](#startAccessCache-int-) | Starts the session that uses caches to access data. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | Unprotects a workbook. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | Unprotects a shared workbook. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class. The default file format type is Xlsx. To create other format file type, please use Workbook(FileFormatType).

```
Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class. The default file format type is Excel97To2003.

```
Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileFormatType | int | The new file format. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class and open a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.lang.String | The file name. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class and open a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class and open a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.lang.String | The file name. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | The load options |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


Initializes a new instance of the [Workbook](../../com.aspose.cells/workbook) class and open stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | The load options |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


Accepts all tracked changes in the workbook.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). Only support adding Xmldsig Digital Signature to an OOXML spreadsheet file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calculates the result of formulas. For all supported formulas, please see the list at https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


Calculates the result of formulas.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |

### calculateFormula(boolean ignoreError, ICustomFunction customFunction) {#calculateFormula-boolean-com.aspose.cells.ICustomFunction-}
```
public void calculateFormula(boolean ignoreError, ICustomFunction customFunction)
```


Calculates the result of formulas. NOTE: This member is now obsolete. Instead, please use CalculateFormula(CalculationOptions) method. This method will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |
| customFunction | [ICustomFunction](../../com.aspose.cells/icustomfunction) | The custom formula calculation functions to extend the calculation engine. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


Calculating formulas in this workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Options for calculation |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


Changes the palette for the spreadsheet in the specified index.

The palette has 56 entries, each represented by an RGB value.

If you set a color which is not in the palette, it will not take effect.

So if you want to set a custom color, please change the palette at first.

The following is the standard color palette.

    | ------- | --- | ----- | ---- |
    | Color   | Red | Green | Blue |
    | Black   | 0   | 0     | 0    |
    | White   | 255 | 255   | 255  |
    | Red     | 255 | 0     | 0    |
    | Lime    | 0   | 255   | 0    |
    | Blue    | 0   | 0     | 255  |
    | Yellow  | 255 | 255   | 0    |
    | Magenta | 255 | 0     | 255  |
    | Cyan    | 0   | 255   | 255  |
    | Maroon  | 128 | 0     | 0    |
    | Green   | 0   | 128   | 0    |
    | Navy    | 0   | 0     | 128  |
    | Olive   | 128 | 128   | 0    |
    | Purple  | 128 | 0     | 128  |
    | Teal    | 0   | 128   | 128  |
    | Silver  | 192 | 192   | 192  |
    | Gray    | 128 | 128   | 128  |
    | Color17 | 153 | 153   | 255  |
    | Color18 | 153 | 51    | 102  |
    | Color19 | 255 | 255   | 204  |
    | Color20 | 204 | 255   | 255  |
    | Color21 | 102 | 0     | 102  |
    | Color22 | 255 | 128   | 128  |
    | Color23 | 0   | 102   | 204  |
    | Color24 | 204 | 204   | 255  |
    | Color25 | 0   | 0     | 128  |
    | Color26 | 255 | 0     | 255  |
    | Color27 | 255 | 255   | 0    |
    | Color28 | 0   | 255   | 255  |
    | Color29 | 128 | 0     | 128  |
    | Color30 | 128 | 0     | 0    |
    | Color31 | 0   | 128   | 128  |
    | Color32 | 0   | 0     | 255  |
    | Color33 | 0   | 204   | 255  |
    | Color34 | 204 | 255   | 255  |
    | Color35 | 204 | 255   | 204  |
    | Color36 | 255 | 255   | 153  |
    | Color37 | 153 | 204   | 255  |
    | Color38 | 255 | 153   | 204  |
    | Color39 | 204 | 153   | 255  |
    | Color40 | 255 | 204   | 153  |
    | Color41 | 51  | 102   | 255  |
    | Color42 | 51  | 204   | 204  |
    | Color43 | 153 | 204   | 0    |
    | Color44 | 255 | 204   | 0    |
    | Color45 | 255 | 153   | 0    |
    | Color46 | 255 | 102   | 0    |
    | Color47 | 102 | 102   | 153  |
    | Color48 | 150 | 150   | 150  |
    | Color49 | 0   | 51    | 102  |
    | Color50 | 51  | 153   | 102  |
    | Color51 | 0   | 51    | 0    |
    | Color52 | 51  | 51    | 0    |
    | Color53 | 153 | 51    | 0    |
    | Color54 | 153 | 51    | 102  |
    | Color55 | 51  | 51    | 153  |
    | Color56 | 51  | 51    | 51   |

    |

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Color structure. |
| index | int | Palette index, 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Closes the session that uses caches to access data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | int | options of data access |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


Combines another Workbook object. Currently, only cell data and cell style of the second Workbook object can be combined. Images, charts and other drawing objects are not supported.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | Another Workbook object. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


Copies data from a source Workbook object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Source Workbook object. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


Copies data from a source Workbook object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Source Workbook object. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


Copies the theme from another workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Source workbook. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


Creates built-in style by given type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int |  |

**Returns:**
[Style](../../com.aspose.cells/style) - style object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


Creates a [CellsColor](../../com.aspose.cells/cellscolor) object.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


Creates a new style.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


Customs the theme. The length of colors should be 12.

    | ----------- | ------------------ |
    | Array index | Theme type         |
    | 0           | Backgournd1        |
    | 1           | Text1              |
    | 2           | Backgournd2        |
    | 3           | Text2              |
    | 4           | Accent1            |
    | 5           | Accent2            |
    | 6           | Accent3            |
    | 7           | Accent4            |
    | 8           | Accent5            |
    | 9           | Accent6            |
    | 10          | Hyperlink          |
    | 11          | Followed Hyperlink |

    |

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| themeName | java.lang.String | The theme name |
| colors | [Color\[\]](../../com.aspose.cells/color) | The theme colors |

### dispose() {#dispose--}
```
public void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


Export XML data linked by the specified XML map.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | java.lang.String | name of the XML map that need to be exported |
| stream | java.io.OutputStream | the export stream |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


Export XML data linked by the specified XML map.

```
Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mapName | java.lang.String | name of the XML map that need to be exported |
| path | java.lang.String | the export path |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


the absolute path of the file. Only used for external links.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) collection that represents all the built-in document properties of the spreadsheet. A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list:

Title

Subject

Author

Keywords

Comments

Template

Last Author

Revision Number

Application Name

Last Print Date

Creation Date

Last Save Time

Total Editing Time

Number of Pages

Number of Words

Number of Characters

Security

Category

Format

Manager

Company

Number of Bytes

Number of Lines

Number of Paragraphs

Number of Slides

Number of Notes

Number of Hidden Slides

Number of Multimedia Clips

```
Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


Gets the factory for building ICellsDataTable from custom objects

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


Returns colors in the palette for the spreadsheet. The palette has 56 entries, each represented by an RGB value.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


Gets the list of [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) objects in the workbook.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


Gets number of the styles in the style pool.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) collection that represents all the custom document properties of the spreadsheet.

```
Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


Represents a Custom XML Data Storage Part (custom XML data within a package).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


Gets the [ExternalConnection](../../com.aspose.cells/externalconnection) collection.

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


Gets mashup data.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


Gets a DataSorter object to sort data.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


the default [Style](../../com.aspose.cells/style) object of the workbook. The DefaultStyle property is useful to implement a Style for the whole Workbook.

```
Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


Gets digital signature from file.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


the file format.

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


the current file name. If the file is opened by stream and there are some external formula references, please set the file name.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


Gets all fonts in the style pool.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


the interrupt monitor.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


Find best matching Color in current palette.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | Raw color. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


Gets the named style in the style pool.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | name of the style |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


the XML file that defines the Ribbon UI.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


Represents the workbook settings.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells. If the returned style is changed, the style of all cells(which refers to this style) will be changed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


Gets the theme name.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


Gets theme color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | The theme color type. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


Gets the [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) in a spreadsheet.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


Gets the [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection in the spreadsheet.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


Indicates whether this workbook contains external links to other data sources. NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Count to check whether there are external links in this workbook. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean - Whether this workbook contains external links to other data sources.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


Indicates if this spreadsheet contains macro/VBA.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


Gets if the workbook has any tracked changes

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


Imports/Updates an XML data file into the workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the xml file stream. |
| sheetName | java.lang.String | the destination sheet name. |
| row | int | the destination row. |
| col | int | the destination column. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


Imports/Updates an XML data file into the workbook.

```
Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| url | java.lang.String | the url/path of the xml file. |
| sheetName | java.lang.String | the destination sheet name. |
| row | int | the destination row |
| col | int | the destination column |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


Checks if a color is in the palette for the spreadsheet.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Color structure. |

**Returns:**
boolean - Returns true if this color is in the palette. Otherwise, returns false
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


Indicates if this spreadsheet is digitally signed.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


Indicates whether license is set.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


Indicates whether structure or window is protected with password.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


Parses all formulas which have not been parsed when they were loaded from template file or set to a cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ignoreError | boolean | whether ignore error for invalid formula. For one invalid formula, if ignore error then this formula will be ignored and the process will continue to parse other formulas, otherwise exception will be thrown. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


Protects a workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| protectionType | int | Protection type. |
| password | java.lang.String | Password to protect the workbook. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


Protects a shared workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password to protect the workbook. |

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculate | boolean | Whether calculates and updates cell values for those dynamic array formulas |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | The options for calculating formulas |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


Removes digital signature from this spreadsheet.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


Removes all external links in the workbook. NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Clear() method. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


Removes VBA/macro from this spreadsheet.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


Removes personal information.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


Remove all unused styles.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


Replaces cells' values with new data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | boolean | The boolean value to be replaced. |
| newValue | java.lang.Object | New value. Can be string, integer, double or DateTime value. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


Replaces cells' values with new data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| intValue | int | The integer value to be replaced. |
| newValue | java.lang.Object | New value. Can be string, integer, double or DateTime value. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


Replaces a cell's value with a new double.

```
Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Cell placeholder |
| newValue | double | Double value to replace |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


Replaces cells' values with a double array.

```
Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Cell placeholder |
| newValues | double[] | Double array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


Replaces a cell's value with a new integer.

```
Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Cell placeholder |
| newValue | int | Integer value to replace |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


Replaces cells' values with an integer array.

```
Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Cell placeholder |
| newValues | int[] | Integer array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


Replaces a cell's value with a new string.

```
Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Cell placeholder |
| newValue | java.lang.String | String value to replace |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


Replaces a cell's value with a new string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Cell placeholder |
| newValue | java.lang.String | String value to replace |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | The replace options |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


Replaces a cell's value with a new string array.

```
Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | java.lang.String | Cell placeholder |
| newValues | java.lang.String[] | String array to replace |
| isVertical | boolean | True - Vertical, False - Horizontal |

**Returns:**
int
### save(InputStream stream, SaveOptions saveOptions) {#save-java.io.InputStream-com.aspose.cells.SaveOptions-}
```
public void save(InputStream stream, SaveOptions saveOptions)
```


Saves the workbook to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The file stream. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | The save options. |

### save(InputStream stream, int saveFormat) {#save-java.io.InputStream-int-}
```
public void save(InputStream stream, int saveFormat)
```


Saves the workbook to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The file stream. |
| saveFormat | int | The save file format type. |

### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


Save the workbook to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The file stream. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | The save options. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


Save the workbook to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The file stream. |
| saveFormat | int | The save file format type. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Save the workbook to the disk.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


Saves the workbook to the disk.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | The save options. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


Saves the workbook to the disk.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| saveFormat | int | The save format type. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


For the description of this property, please see [getAbsolutePath()](../../com.aspose.cells/workbook\#getAbsolutePath--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


For the description of this property, please see [getDefaultStyle()](../../com.aspose.cells/workbook\#getDefaultStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Sets digital signature to an spreadsheet file (Excel2007 and later). Only support adding Xmldsig Digital Signature

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


Set Encryption Options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| encryptionType | int | The encryption type. |
| keyLength | int | The key length. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


For the description of this property, please see [getFileFormat()](../../com.aspose.cells/workbook\#getFileFormat--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


For the description of this property, please see [getFileName()](../../com.aspose.cells/workbook\#getFileName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


For the description of this property, please see [getInterruptMonitor()](../../com.aspose.cells/workbook\#getInterruptMonitor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


For the description of this property, please see [getRibbonXml()](../../com.aspose.cells/workbook\#getRibbonXml--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


Sets the theme color

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | The theme color type. |
| color | [Color](../../com.aspose.cells/color) | the theme color |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Starts the session that uses caches to access data. If the cache of specified data access requires some data models in worksheet to be "read-only", then corresponding data models in every worksheet in this workbook will be taken as "read-only" and user should not change any of them.

After finishing the access to the data, [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) should be invoked with same options to clear all caches and recover normal access mode.



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | int | options of data access |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Unprotects a workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password to unprotect the workbook. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


Unprotects a shared workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Password to unprotect the workbook. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data. If the method is not called before calculating formulas, Aspose.Cells will use the previous information(cached in the file); Please set CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath. And please set Workbook.FilePath if this workbook is from a stream, otherwise Aspose.Cells could not get the external link full path sometimes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | External workbooks are referenced by this workbook. If it's null, we will directly open the external linked files.. If it's not null, we will check whether the external link in the array first; if not, we will open the external linked files again. |

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

