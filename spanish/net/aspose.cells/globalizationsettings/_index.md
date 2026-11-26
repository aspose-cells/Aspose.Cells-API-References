---
title: "Clase GlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GlobalizationSettings. Representa la configuración de globalización"
type: docs
url: /es/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Representa la configuración de globalización.

```csharp
public class GlobalizationSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Obtiene o establece la configuración de globalización para el gráfico. |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray/) { get; } | Obtiene el separador para los elementos en los datos de fila de la matriz en la fórmula. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator/) { get; } | Obtiene el separador para la lista, los parámetros de la función, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Obtiene o establece la configuración de globalización para la tabla dinámica. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray/) { get; } | Obtiene el separador para las filas en los datos de matriz en la fórmula. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Compara dos valores de cadena según ciertas reglas de ordenación. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "(All)" en la tabla dinámica. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring/)(bool) | Obtiene la cadena de visualización del valor booleano de la celda |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Transforma la cadena en un objeto comparable según ciertas reglas de ordenación. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "Column Labels" en la tabla dinámica. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename/)(CommentTitleType) | Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título de comentario. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Obtiene el nombre del encabezado del campo de área de valores en la tabla dinámica. |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Obtiene el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente. El valor predeterminado es "Sheet". |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "(blank)" en la tabla dinámica. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring/)(string) | Obtiene la cadena de visualización del valor de error de la celda |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Obtiene el nombre del total general de la función. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname/)(string) | Obtiene el texto dependiente de la configuración regional para el Nombre incorporado según el texto estándar proporcionado. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname/)(string) | Obtiene el nombre de la función dependiente de la configuración regional según el nombre estándar de la función proporcionado. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "(Multiple Items)" en la tabla dinámica. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "Grand Total" en la tabla dinámica. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "Total" en la tabla dinámica. Necesita sobrescribir este método cuando la tabla dinámica contiene dos o más PivotFields en el área de datos. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Obtiene el nombre de protección en la tabla dinámica. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "Row Labels" en la tabla dinámica. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname/)(string) | Obtiene el texto estándar del Nombre incorporado según el texto dependiente de la configuración regional proporcionado. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname/)(string) | Obtiene el nombre estándar de la función según el nombre de función dependiente de la configuración regional proporcionado. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/)(string) | Obtiene el nombre de estilo de fuente estándar en inglés (Regular, Bold, Italic) para Encabezado/Pie de página según el nombre de estilo de fuente dependiente de la configuración regional proporcionado. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Obtiene el nombre del tipo [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) en la tabla dinámica. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall/)() | Obtiene el nombre del tipo de filas de tabla que consiste en todas las filas de la tabla referenciada. El valor predeterminado es "All", por lo que en la fórmula "#All" representa todas las filas de la tabla referenciada. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent/)() | Obtiene el nombre del tipo de filas de tabla que consiste en la fila actual de la tabla referenciada. El valor predeterminado es "This Row", por lo que en la fórmula "#This Row" representa la fila actual de la tabla referenciada. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata/)() | Obtiene el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada. El predeterminado es "Data", por lo que en la fórmula "#Data" representa la región de datos de la tabla. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders/)() | Obtiene el nombre del tipo de filas de tabla que consiste en el encabezado de la tabla. El predeterminado es "Headers", por lo que en la fórmula "#Headers" representa el encabezado de la tabla. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals/)() | Obtiene el nombre del tipo de filas de tabla que consiste en la fila total de la tabla referenciada. El valor predeterminado es "Totals", por lo que en la fórmula "#Totals" representa la fila total de la tabla referenciada. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname/)(ConsolidationFunction) | Obtiene el nombre total de la función. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].PutValue("Region");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("North");
            cells["B2"].PutValue(1000);
            cells["A3"].PutValue("South");
            cells["B3"].PutValue(2000);
            cells["A4"].PutValue("East");
            cells["B4"].PutValue(3000);
            cells["A5"].PutValue("West");
            cells["B5"].PutValue(4000);

            // Crear y aplicar configuraciones de globalización
            GlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Aplicar subtotal con globalización personalizada
            CellArea area = CellArea.CreateCellArea(0, 0, 5, 1);
            cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 0 }, true, false, true);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTotalName(ConsolidationFunction functionType)
        {
            // Personalizar el nombre total según el tipo de función
            switch (functionType)
            {
                case ConsolidationFunction.Sum:
                    return "Custom Sum";
                case ConsolidationFunction.Count:
                    return "Custom Count";
                default:
                    return base.GetTotalName(functionType);
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


