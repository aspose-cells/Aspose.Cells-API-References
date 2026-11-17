---
title: "Clase TxtLoadOptions"
linktitle: "TxtLoadOptions"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase TxtLoadOptions. Encapsula el objeto que representa txtloadoptions en Go."
type: docs
weight: 200
url: /es/go-cpp/txtloadoptions/
---

## TxtLoadOptions class

Represents the options for loading text file.

```go

type TxtLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewTxtLoadOptions](./newtxtloadoptions/) | Crea las opciones para cargar un archivo de texto. |
| [NewTxtLoadOptions_LoadFormat](./newtxtloadoptions_loadformat/) | Crea las opciones para cargar un archivo de texto. |
| [NewTxtLoadOptions_AbstractTextLoadOptions](./newtxtloadoptions_abstracttextloadoptions/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetSeparator](./getseparator/) | Obtiene y establece el separador de caracteres del archivo de texto. |
| [SetSeparator](./setseparator/) | Obtiene y establece el separador de caracteres del archivo de texto. |
| [GetSeparatorString](./getseparatorstring/) | Obtiene y establece un valor de cadena como separador. |
| [SetSeparatorString](./setseparatorstring/) | Obtiene y establece un valor de cadena como separador. |
| [IsMultiEncoded](./ismultiencoded/) | True indica que el archivo contiene varias codificaciones. |
| [SetIsMultiEncoded](./setismultiencoded/) | True indica que el archivo contiene varias codificaciones. |
| [GetHasFormula](./gethasformula/) | Indicates whether the text is formula if it starts with "=". |
| [SetHasFormula](./sethasformula/) | Indicates whether the text is formula if it starts with "=". |
| [GetHasTextQualifier](./gethastextqualifier/) | Indica si hay calificador de texto para el valor de la celda. El valor predeterminado es true. |
| [SetHasTextQualifier](./sethastextqualifier/) | Indica si hay calificador de texto para el valor de la celda. El valor predeterminado es true. |
| [GetTextQualifier](./gettextqualifier/) | Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'. |
| [SetTextQualifier](./settextqualifier/) | Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'. |
| [GetTreatConsecutiveDelimitersAsOne](./gettreatconsecutivedelimitersasone/) | Indica si los delimitadores consecutivos deben tratarse como uno. |
| [SetTreatConsecutiveDelimitersAsOne](./settreatconsecutivedelimitersasone/) | Indica si los delimitadores consecutivos deben tratarse como uno. |
| [GetTreatQuotePrefixAsValue](./gettreatquoteprefixasvalue/) | Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es true. Si es false, la comilla simple inicial se eliminará del valor de la celda correspondiente y Style.QuotePrefix se establecerá como true para la celda. |
| [SetTreatQuotePrefixAsValue](./settreatquoteprefixasvalue/) | Indica si el signo de comilla simple inicial debe tomarse como parte del valor de una celda. El valor predeterminado es true. Si es false, la comilla simple inicial se eliminará del valor de la celda correspondiente y Style.QuotePrefix se establecerá como true para la celda. |
| [GetExtendToNextSheet](./getextendtonextsheet/) | Indica si se extienden los datos a la hoja siguiente cuando las filas o columnas de datos exceden el límite. El valor predeterminado es false. |
| [SetExtendToNextSheet](./setextendtonextsheet/) | Indica si se extienden los datos a la hoja siguiente cuando las filas o columnas de datos exceden el límite. El valor predeterminado es false. |
| [GetHeaderRowsCount](./getheaderrowscount/) | El recuento de filas de encabezado que se repetirán en hojas extendidas. |
| [SetHeaderRowsCount](./setheaderrowscount/) | El recuento de filas de encabezado que se repetirán en hojas extendidas. |
| [GetHeaderColumnsCount](./getheadercolumnscount/) | El recuento de columnas de encabezado que se repetirán en hojas extendidas. |
| [SetHeaderColumnsCount](./setheadercolumnscount/) | El recuento de columnas de encabezado que se repetirán en hojas extendidas. |
| [GetMaxRowCount](./getmaxrowcount/) | El recuento máximo de filas que se importarán para una hoja. |
| [SetMaxRowCount](./setmaxrowcount/) | El recuento máximo de filas que se importarán para una hoja. |
| [GetMaxColumnCount](./getmaxcolumncount/) | El recuento máximo de columnas que se importarán para una hoja. |
| [SetMaxColumnCount](./setmaxcolumncount/) | El recuento máximo de columnas que se importarán para una hoja. |
| [GetEncoding](./getencoding/) | Gets and sets the default encoding. Only applies for csv file. |
| [SetEncoding](./setencoding/) | Gets and sets the default encoding. Only applies for csv file. |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [GetConvertNumericData](./getconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data.Default value is true. |
| [SetConvertNumericData](./setconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data.Default value is true. |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data.Default value is true. |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data.Default value is true. |
| [GetKeepPrecision](./getkeepprecision/) | Indicates whether not parsing a string value if the length is 15. |
| [SetKeepPrecision](./setkeepprecision/) | Indicates whether not parsing a string value if the length is 15. |
| [GetLoadFormat](./getloadformat/) | Gets the load format. |
| [GetPassword](./getpassword/) | Gets and set the password of the workbook. |
| [SetPassword](./setpassword/) | Gets and set the password of the workbook. |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file.The default value is false. |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file.The default value is false. |
| [SetPaperSize](./setpapersize/) | Sets the default print paper size from default printer's setting. |
| [GetLanguageCode](./getlanguagecode/) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [SetLanguageCode](./setlanguagecode/) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [GetRegion](./getregion/) | Gets or sets the regional settings used for the Workbook that will be loaded. |
| [SetRegion](./setregion/) | Gets or sets the regional settings used for the Workbook that will be loaded. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Gets the default style settings for initializing styles of the workbook |
| [GetInterruptMonitor](./getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [SetInterruptMonitor](./setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | Ignore the data which are not printed if directly printing the file |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | Ignore the data which are not printed if directly printing the file |
| [GetCheckDataValid](./getcheckdatavalid/) | Check whether data is valid in the template file. |
| [SetCheckDataValid](./setcheckdatavalid/) | Check whether data is valid in the template file. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.If this property is false, we will accept your input string value as the cell's value so that lateryou can output the complete string value for other file formats such as CSV.However, if you have set such kind of value that is invalid for excel file format,you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.If this property is false, we will accept your input string value as the cell's value so that lateryou can output the complete string value for other file formats such as CSV.However, if you have set such kind of value that is invalid for excel file format,you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [GetKeepUnparsedData](./getkeepunparseddata/) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [SetKeepUnparsedData](./setkeepunparseddata/) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [GetLoadFilter](./getloadfilter/) | The filter to denote how to load data. |
| [SetLoadFilter](./setloadfilter/) | The filter to denote how to load data. |
| [GetMemorySetting](./getmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [SetMemorySetting](./setmemorysetting/) | Gets or sets the memory mode for loaded workbook. |
| [GetAutoFitterOptions](./getautofitteroptions/) | Gets and sets the auto fitter options |
| [SetAutoFitterOptions](./setautofitteroptions/) | Gets and sets the auto fitter options |
| [GetAutoFilter](./getautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [SetAutoFilter](./setautofilter/) | Indicates whether auto filtering the data when loading the files. |
| [GetFontConfigs](./getfontconfigs/) | Gets and sets individual font configs.Only works for the Workbook which uses this LoadOptions to load. |
| [SetFontConfigs](./setfontconfigs/) | Gets and sets individual font configs.Only works for the Workbook which uses this LoadOptions to load. |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | Indicates whether ignoring useless shapes. |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokenswhile getting and setting formulas.Default value is false. |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokenswhile getting and setting formulas.Default value is false. |
