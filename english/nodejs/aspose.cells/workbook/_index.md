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
| [acceptAllRevisions()](./acceptallrevisions/) | Accepts all tracked changes in the workbook. |
| [addDigitalSignature(digitalSignatureCollection)](./adddigitalsignature/) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). Only support adding Xmldsig Digital Signature |
| [calculateFormula()](./calculateformula/) | Calculates the result of formulas. For all supported formulas, please see the list at https://docs.aspose.com/display/ce |
| [calculateFormula(ignoreError)](./calculateformula-1/) | Calculates the result of formulas. |
| [calculateFormula(options)](./calculateformula-2/) | Calculating formulas in this workbook. |
| [changePalette(color, index)](./changepalette/) | Changes the palette for the spreadsheet in the specified index. The palette has 56 entries, each represented by an RGB v |
| [closeAccessCache(opts)](./closeaccesscache/) | Closes the session that uses caches to access data. |
| [combine(secondWorkbook)](./combine/) | Combines another Workbook object. Merge Excel, ODS , CSV and other files to one file. |
| [constructor_overload$1(fileFormatType)](./constructor-overload1/) | Initializes a new instance of the Workbook class. The default file format type is Excel97To2003. |
| [constructor_overload$2()](./constructor-overload2/) |  |
| [constructor_overload$3(file)](./constructor-overload3/) | Initializes a new instance of the Workbook class and open a file. |
| [constructor_overload$4(file, loadOptions)](./constructor-overload4/) | Initializes a new instance of the Workbook class and open a file. |
| [copy(source, copyOptions)](./copy/) | Copies another Workbook object. It's very simple to clone an Excel file. |
| [copy(source)](./copy-1/) | Copies data from a source Workbook object. |
| [copyTheme(source)](./copytheme/) | Copies the theme from another workbook. |
| [createBuiltinStyle(type)](./createbuiltinstyle/) | Creates built-in style by given type. |
| [createCellsColor()](./createcellscolor/) | Creates a CellsColor object. |
| [createStyle()](./createstyle/) | Creates a new style. |
| [createStyle()](./createstyle-1/) |  |
| [customTheme(themeName, colors)](./customtheme/) | Customs the theme. The length of colors should be 12. Array indexTheme type0Backgournd11Text12Backgournd23Text24Accent15 |
| [dispose()](./dispose/) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [exportXml(mapName, path)](./exportxml/) | Export XML data linked by the specified XML map. |
| [exportXml(mapName, stream)](./exportxml-1/) | Export XML data linked by the specified XML map. |
| [getAbsolutePath()](./getabsolutepath/) | Gets and sets the absolute path of the file. Only used for external links. |
| [getBuiltInDocumentProperties()](./getbuiltindocumentproperties/) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new pro |
| [getCellsDataTableFactory()](./getcellsdatatablefactory/) | Gets the factory for building ICellsDataTable from custom objects |
| [getColors()](./getcolors/) | Returns colors in the palette for the spreadsheet. The palette has 56 entries, each represented by an RGB value. |
| [getContentTypeProperties()](./getcontenttypeproperties/) | Gets the list of ContentTypeProperty objects in the workbook. |
| [getCountOfStylesInPool()](./getcountofstylesinpool/) | Gets number of the styles in the style pool. |
| [getCustomDocumentProperties()](./getcustomdocumentproperties/) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [getCustomXmlParts()](./getcustomxmlparts/) | Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [getDataConnections()](./getdataconnections/) | Gets the ExternalConnection collection. |
| [getDataMashup()](./getdatamashup/) | Gets mashup data. |
| [getDataModel()](./getdatamodel/) |  |
| [getDataSorter()](./getdatasorter/) | Gets a DataSorter object to sort data. |
| [getDefaultStyle()](./getdefaultstyle/) | Gets or sets the default Style object of the workbook. The DefaultStyle property is useful to implement a Style for the  |
| [getDigitalSignature()](./getdigitalsignature/) | Gets digital signature from file. |
| [getFileFormat()](./getfileformat/) | Gets and sets the file format. The value of the property is FileFormatType integer constant. |
| [getFileName()](./getfilename/) | Gets and sets the current file name. If the file is opened by stream and there are some external formula references, ple |
| [getFonts()](./getfonts/) | Gets all fonts in the style pool. |
| [getInterruptMonitor()](./getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [getMatchingColor(rawColor)](./getmatchingcolor/) | Find best matching Color in current palette. |
| [getNamedStyle(name)](./getnamedstyle/) | Gets the named style in the style pool. |
| [getRibbonXml()](./getribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. |
| [getSettings()](./getsettings/) | Represents the workbook settings. |
| [getStyleInPool(index)](./getstyleinpool/) | Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple refere |
| [getTheme()](./gettheme/) | Gets the theme name. |
| [getThemeColor(type)](./getthemecolor/) | Gets theme color. |
| [getVbaProject()](./getvbaproject/) | Gets the VbaProject in a spreadsheet. |
| [getWorksheets()](./getworksheets/) | Gets the WorksheetCollection collection in the spreadsheet. |
| [hasCustomFunction()](./hascustomfunction/) |  |
| [hasExernalLinks()](./hasexernallinks/) | Indicates whether this workbook contains external links to other data sources. NOTE: This member is now obsolete. Instea |
| [hasMacro()](./hasmacro/) | Indicates if this spreadsheet contains macro/VBA. |
| [hasRevisions()](./hasrevisions/) | Gets if the workbook has any tracked changes |
| [importXml(url, sheetName, row, col)](./importxml/) | Imports/Updates an XML data file into the workbook. |
| [importXml(stream, sheetName, row, col)](./importxml-1/) | Imports/Updates an XML data file into the workbook. |
| [isColorInPalette(color)](./iscolorinpalette/) | Checks if a color is in the palette for the spreadsheet. |
| [isDigitallySigned()](./isdigitallysigned/) | Indicates if this spreadsheet is digitally signed. |
| [isLicensed()](./islicensed/) | Indicates whether license is set. |
| [isWorkbookProtectedWithPassword()](./isworkbookprotectedwithpassword/) | Indicates whether structure or window is protected with password. |
| [mergeNamedStyles()](./mergenamedstyles/) |  |
| [parseFormulas(ignoreError)](./parseformulas/) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [protect(protectionType, password)](./protect/) | Protects a workbook. |
| [protectSharedWorkbook(password)](./protectsharedworkbook/) | Protects a shared workbook. |
| [refreshAll()](./refreshall/) |  |
| [refreshDynamicArrayFormulas(calculate)](./refreshdynamicarrayformulas/) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in  |
| [refreshDynamicArrayFormulas(calculate, copts)](./refreshdynamicarrayformulas-1/) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) For performance co |
| [removeDigitalSignature()](./removedigitalsignature/) | Removes digital signature from this spreadsheet. |
| [removeExternalLinks()](./removeexternallinks/) | Removes all external links in the workbook. NOTE: This member is now obsolete. Instead, please use ExternalLinkCollectio |
| [removeMacro()](./removemacro/) | Removes VBA/macro from this spreadsheet. |
| [removePersonalInformation()](./removepersonalinformation/) | Removes personal information. |
| [removeUnusedStyles()](./removeunusedstyles/) | Remove all unused styles. |
| [replace(placeHolder, newValue)](./replace/) | Replaces a cell's value with a new string. |
| [replace(placeHolder, newValue)](./replace-1/) | Replaces a cell's value with a new integer. |
| [replace(placeHolder, newValue)](./replace-2/) | Replaces a cell's value with a new double. |
| [replace(placeHolder, newValues, isVertical)](./replace-3/) | Replaces a cell's value with a new string array. |
| [replace(placeHolder, newValue, options)](./replace-4/) | Replaces a cell's value with a new string. |
| [save(fileName, saveFormat)](./save/) | Saves the workbook to the disk. |
| [save(fileName)](./save-1/) | Save the workbook to the disk. |
| [save(fileName, saveOptions)](./save-2/) | Saves the workbook to the disk. |
| [setAbsolutePath()](./setabsolutepath/) | Gets and sets the absolute path of the file. Only used for external links. |
| [setDefaultStyle()](./setdefaultstyle/) | Gets or sets the default Style object of the workbook. The DefaultStyle property is useful to implement a Style for the  |
| [setDigitalSignature(digitalSignatureCollection)](./setdigitalsignature/) | Sets digital signature to an spreadsheet file (Excel2007 and later). Only support adding Xmldsig Digital Signature |
| [setEncryptionOptions(encryptionType, keyLength)](./setencryptionoptions/) | Set Encryption Options. |
| [setFileFormat()](./setfileformat/) | Gets and sets the file format. The value of the property is FileFormatType integer constant. |
| [setFileName()](./setfilename/) | Gets and sets the current file name. If the file is opened by stream and there are some external formula references, ple |
| [setInterruptMonitor()](./setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [setRibbonXml()](./setribbonxml/) | Gets and sets the XML file that defines the Ribbon UI. |
| [setThemeColor(type, color)](./setthemecolor/) | Sets the theme color |
| [startAccessCache(opts)](./startaccesscache/) | Starts the session that uses caches to access data. If the cache of specified data access requires some data models in w |
| [unprotect(password)](./unprotect/) | Unprotects a workbook. |
| [unprotectSharedWorkbook(password)](./unprotectsharedworkbook/) | Unprotects a shared workbook. |
| [updateCustomFunctionDefinition(definition)](./updatecustomfunctiondefinition/) | Updates definition of custom functions. This method can be used for some special scenarios. For example, if user needs s |
| [updateLinkedDataSource(externalWorkbooks)](./updatelinkeddatasource/) | If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data fro |
| [createWorkbookFromStream(stream, callback)](./createworkbookfromstream/) *(static)* | Initializes a new instance of the Workbook class and open a stream. |
| [createWorkbookFromStream(stream, loadOptions, callback)](./createworkbookfromstream-1/) *(static)* | Initializes a new instance of the Workbook class and open a stream. |
| [save(workbook, stream, saveOptions)](./save-3/) *(static)* | Save the workbook to the stream. |
| [save(workbook, stream, saveFormat)](./save-4/) *(static)* | Save the workbook to the stream. |
