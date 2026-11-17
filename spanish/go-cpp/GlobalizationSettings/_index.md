---
title: "Clase GlobalizationSettings"
linktitle: "GlobalizationSettings"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase GlobalizationSettings. Encapsula el objeto que representa globalizationsettings en Go."
type: docs
weight: 200
url: /es/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

Represents the globalization settings.

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | Default constructor. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetChartSettings](./getchartsettings/) | Obtiene la configuración de globalización para Chart. |
| [SetChartSettings](./setchartsettings/) | Establece la configuración de globalización para Chart. |
| [GetPivotSettings](./getpivotsettings/) | Obtiene la configuración de globalización para la tabla dinámica. |
| [SetPivotSettings](./setpivotsettings/) | Establece la configuración de globalización para la tabla dinámica. |
| [GetTotalName](./gettotalname/) | Obtiene el nombre total de la función. |
| [GetGrandTotalName](./getgrandtotalname/) | Gets the grand total name of the function. |
| [GetDefaultSheetName](./getdefaultsheetname/) | Obtiene el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente. El predeterminado es "Sheet". |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Gets the type name of table rows that consists of the table header.Default is "Headers", so in formula "#Headers" represents the table header. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Gets the type name of table rows that consists of data region of referenced table.Default is "Data", so in formula "#Data" represents the data region of the table. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Obtiene el nombre de tipo de filas de tabla que consiste en todas las filas de la tabla referenciada. El predeterminado es "All", por lo que en la fórmula "#All" representa todas las filas de la tabla referenciada. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Obtiene el nombre de tipo de filas de tabla que consiste en la fila total de la tabla referenciada. El predeterminado es "Totals", por lo que en la fórmula "#Totals" representa la fila total de la tabla referenciada. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Obtiene el nombre de tipo de filas de tabla que consiste en la fila actual de la tabla referenciada. El predeterminado es "This Row", por lo que en la fórmula "#This Row" representa la fila actual de la tabla referenciada. |
| [GetErrorValueString](./geterrorvaluestring/) | Gets the display string value for cell's error value |
| [GetBooleanValueString](./getbooleanvaluestring/) | Gets the display string value for cell's boolean value |
| [GetLocalFunctionName](./getlocalfunctionname/) | Gets the locale dependent function name according to given standard function name. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Gets the standard function name according to given locale dependent function name. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Gets the locale dependent text for built-in Name according to given standard text. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Gets the standard text of built-in Name according to given locale dependent text. |
| [GetListSeparator](./getlistseparator/) | Gets the separator for list, parameters of function, ...etc. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Gets the separator for rows in array data in formula. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Gets the separator for the items in array's row data in formula. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Gets standard English font style name(Regular, Bold, Italic) for Header/Footer according to given locale font style name. |
| [GetCommentTitleName](./getcommenttitlename/) | Gets the locale dependent comment title name according to comment title type. |
| [Compare](./compare/) | Compara dos valores de cadena según ciertas reglas de ordenación. |
