---
title: GlobalizationSettings
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la configuración de globalización.
type: docs
weight: 3620
url: /es/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Representa la configuración de globalización.

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | Obtiene o establece el gráfico de este[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | Obtiene el separador de los elementos en los datos de la fila de la matriz en la fórmula. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | Obtiene el separador de lista, parámetros de función, etc. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | Obtiene el separador de filas en datos de matriz en fórmula. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | Compara dos valores de cadena de acuerdo con ciertas reglas de intercalación. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | Obtiene el nombre de la etiqueta "(Todos)" en la tabla dinámica. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | Obtiene el valor de cadena de visualización para el valor booleano de la celda |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | Transforma la cadena en un objeto comparable según ciertas reglas de clasificación. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | Obtiene el nombre de la etiqueta "Etiquetas de columna" en la tabla dinámica. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | Obtiene el nombre del título del comentario que depende de la configuración regional según el tipo de título del comentario. |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | Obtiene el nombre de la etiqueta "(en blanco)" en la tabla dinámica. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | Obtiene el valor de cadena de visualización para el valor de error de la celda |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | Obtiene el nombre total general de la función. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | Obtiene el texto dependiente de la configuración regional para el nombre integrado de acuerdo con el texto estándar proporcionado. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | Obtiene el nombre de la función dependiente de la configuración regional de acuerdo con el nombre de función estándar dado. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | Obtiene el nombre de la etiqueta "(Múltiples elementos)" en la tabla dinámica. |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | Obtiene el nombre de las etiquetas "Otros" para gráficos circulares. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | Obtiene el nombre de la etiqueta "Total general" en la tabla dinámica. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | Obtiene el nombre de la etiqueta "Total" en la tabla dinámica. Debe invalidar este método cuando la tabla dinámica contiene dos o más campos dinámicos en el área de datos. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | Obtiene el nombre de la protección en la tabla dinámica. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | Obtiene el nombre de la etiqueta "Row Labels" en la tabla dinámica. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | Obtiene el texto estándar del Nombre integrado de acuerdo con el texto dependiente de la configuración regional dado. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | Obtiene el nombre de función estándar de acuerdo con el nombre de función dependiente de la configuración regional dado. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | Obtiene el nombre de estilo de fuente estándar en inglés (regular, negrita, cursiva) para encabezado/pie de página de acuerdo con el nombre de estilo de fuente de la configuración regional dada. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | Obtiene el nombre de[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) escriba en la tabla dinámica. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | Obtiene el nombre de tipo de las filas de la tabla que consta de todas las filas de la tabla a la que se hace referencia. El valor predeterminado es "Todos", por lo que en la fórmula "#Todas" representa todas las filas de la tabla a la que se hace referencia. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | Obtiene el nombre de tipo de las filas de la tabla que consta de la fila actual en la tabla a la que se hace referencia. El valor predeterminado es "Esta fila", por lo que en la fórmula "#Esta fila" representa la fila actual en la tabla a la que se hace referencia. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | Obtiene el nombre de tipo de las filas de la tabla que consta de la región de datos de la tabla a la que se hace referencia. El valor predeterminado es "Data", por lo que en la fórmula "#Data" representa la región de datos de la tabla. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | Obtiene el nombre de tipo de las filas de la tabla que consta del encabezado de la tabla. El valor predeterminado es "Encabezados", por lo que en la fórmula "#Encabezados" representa el encabezado de la tabla. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | Obtiene el nombre de tipo de las filas de la tabla que consta de la fila total de la tabla a la que se hace referencia. El valor predeterminado es "Totales", por lo que en la fórmula "#Totales" representa la fila total de la tabla a la que se hace referencia. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | Obtiene el nombre total de la función. |

### Ver también

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
