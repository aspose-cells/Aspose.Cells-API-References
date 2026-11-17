---
title: "MarkdownSaveOptions Clase"
linktitle: "MarkdownSaveOptions"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "MarkdownSaveOptions clase. Encapsula el objeto que representa markdownsaveoptions en Go."
type: docs
weight: 200
url: /es/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Represents the save options for markdown.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | Crea opciones para guardar documento markdown |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetEncoding](./getencoding/) | Obtiene y establece la codificación predeterminada. |
| [SetEncoding](./setencoding/) | Obtiene y establece la codificación predeterminada. |
| [GetFormatStrategy](./getformatstrategy/) | Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena. |
| [SetFormatStrategy](./setformatstrategy/) | Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena. |
| [GetLineSeparator](./getlineseparator/) | Obtiene y establece el separador de línea. |
| [SetLineSeparator](./setlineseparator/) | Obtiene y establece el separador de línea. |
| [GetTableHeaderType](./gettableheadertype/) | Obtiene y establece cómo establecer el encabezado de la tabla. |
| [SetTableHeaderType](./settableheadertype/) | Obtiene y establece cómo establecer el encabezado de la tabla. |
| [GetSheetSet](./getsheetset/) | Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSheetSet](./setsheetset/) | Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: Aspose.Cells.Rendering.SheetSet.Active. |
| [GetImageOptions](./getimageoptions/) | Get the ImageOrPrintOptions object before exporting |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Especifica si las imágenes se guardan en formato Base64 en Markdown. El valor predeterminado es verdadero. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Especifica si las imágenes se guardan en formato Base64 en Markdown. El valor predeterminado es verdadero. |
| [GetCalculateFormula](./getcalculateformula/) | Indica si se deben calcular las fórmulas antes de guardar el archivo markdown. |
| [SetCalculateFormula](./setcalculateformula/) | Indica si se deben calcular las fórmulas antes de guardar el archivo markdown. |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | Indica si se debe exportar el hipervínculo usando definiciones de referencia en lugar del formato en línea. El valor predeterminado es falso. |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | Indica si se debe exportar el hipervínculo usando definiciones de referencia en lugar del formato en línea. El valor predeterminado es falso. |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | Indica si la alineación de columnas está habilitada para las tablas Markdown generadas. Cuando está habilitada, las columnas se alinean rellenando el contenido de la celda con el carácter especificado (normalmente ' ' para espacios). Establezca "\\0" para desactivar la alineación de columnas (predeterminado). |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | Indica si la alineación de columnas está habilitada para las tablas Markdown generadas. Cuando está habilitada, las columnas se alinean rellenando el contenido de la celda con el carácter especificado (normalmente ' ' para espacios). Establezca "\\0" para desactivar la alineación de columnas (predeterminado). |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | Indica si las filas en blanco en la hoja de cálculo deben tratarse como separadores de tabla al exportar a Markdown. El valor predeterminado es falso. |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | Indica si las filas en blanco en la hoja de cálculo deben tratarse como separadores de tabla al exportar a Markdown. El valor predeterminado es falso. |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | Indica cómo se exportan los objetos OfficeMath a Markdown. El valor predeterminado es Imagen. |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | Indica cómo se exportan los objetos OfficeMath a Markdown. El valor predeterminado es Imagen. |
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
