---
title: "Clase TxtSaveOptions"
linktitle: "TxtSaveOptions"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase TxtSaveOptions. Encapsula el objeto que representa txtsaveoptions en Go."
type: docs
weight: 200
url: /es/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

Represents the save options for csv/tab delimited/other text format.

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | Crea opciones de guardado de archivo de texto. |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | Crea opciones de guardado de archivo de texto. |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetSeparator](./getseparator/) | Obtiene y establece el delimitador de caracteres del archivo de texto. |
| [SetSeparator](./setseparator/) | Obtiene y establece el delimitador de caracteres del archivo de texto. |
| [GetSeparatorString](./getseparatorstring/) | Obtiene y establece un valor de cadena como separador. |
| [SetSeparatorString](./setseparatorstring/) | Obtiene y establece un valor de cadena como separador. |
| [GetEncoding](./getencoding/) | Obtiene y establece la codificación predeterminada. |
| [SetEncoding](./setencoding/) | Obtiene y establece la codificación predeterminada. |
| [GetQuoteType](./getquotetype/) | Obtiene o establece cómo citar los valores en el archivo de texto exportado. |
| [SetQuoteType](./setquotetype/) | Obtiene o establece cómo citar los valores en el archivo de texto exportado. |
| [GetFormatStrategy](./getformatstrategy/) | Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena. |
| [SetFormatStrategy](./setformatstrategy/) | Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena. |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | Indica si las filas y columnas en blanco iniciales deben recortarse como lo hace ms excel. El valor predeterminado es true. |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | Indica si las filas y columnas en blanco iniciales deben recortarse como lo hace ms excel. El valor predeterminado es true. |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | Indica si las celdas en blanco finales en una fila deben recortarse. El valor predeterminado es false. |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | Indica si las celdas en blanco finales en una fila deben recortarse. El valor predeterminado es false. |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | Indica si se deben generar separadores para una fila en blanco. El valor predeterminado es false, por lo que por defecto el contenido de la fila en blanco estará vacío. |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | Indica si se deben generar separadores para una fila en blanco. El valor predeterminado es false, por lo que por defecto el contenido de la fila en blanco estará vacío. |
| [GetExportArea](./getexportarea/) | El rango de celdas a exportar. |
| [SetExportArea](./setexportarea/) | El rango de celdas a exportar. |
| [GetExportQuotePrefix](./getexportquoteprefix/) | Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando Style.QuotePrefix es true para ella. El valor predeterminado es false. |
| [SetExportQuotePrefix](./setexportquoteprefix/) | Indica si el signo de comilla simple debe exportarse como parte del valor de una celda cuando Style.QuotePrefix es true para ella. El valor predeterminado es false. |
| [GetExportAllSheets](./getexportallsheets/) | Indica si se exportan todas las hojas al archivo de texto. Si es false, solo se exporta la hoja activa, al igual que MS Excel. |
| [SetExportAllSheets](./setexportallsheets/) | Indica si se exportan todas las hojas al archivo de texto. Si es false, solo se exporta la hoja activa, al igual que MS Excel. |
| [GetSaveFormat](./getsaveformat/) | Gets the save file format. |
| [GetClearData](./getcleardata/) | Make the workbook empty after saving the file. |
| [SetClearData](./setcleardata/) | Make the workbook empty after saving the file. |
| [GetCachedFileFolder](./getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder](./setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetMergeAreas](./getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetMergeAreas](./setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetCreateDirectory](./getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetCreateDirectory](./setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetSortNames](./getsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetSortNames](./setsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetSortExternalNames](./getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortExternalNames](./setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Indicates whether to cache the latest data of the chart. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Indicates whether to cache the latest data of the chart. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. |
