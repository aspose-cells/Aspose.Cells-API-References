---
title: "Clase SettableGlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.SettableGlobalizationSettings. Implementación de GlobalizationSettings que permite al usuario establecer/cambiar textos predefinidos"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

Implementación de GlobalizationSettings que permite al usuario establecer/cambiar textos predefinidos.

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | Obtiene o establece la configuración de globalización para Chart. (Hereda de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | Obtiene el separador para los elementos en los datos de fila de la matriz en la fórmula. |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | Obtiene el separador para la lista, los parámetros de la función, ...etc. |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | Obtiene o establece la configuración de globalización para la tabla dinámica. (Hereda de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | Obtiene el separador para las filas en los datos de matriz en la fórmula. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | Compara dos valores de cadena según ciertas reglas de ordenación. (Hereda de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "(All)" en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | Obtiene la cadena de visualización del valor booleano de la celda |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | Transforma la cadena en un objeto comparable según ciertas reglas de ordenación.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "Column Labels" en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título de comentario. |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) Obtiene el nombre del encabezado del campo del área de valores en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | Obtiene el nombre de hoja predeterminado para agregar la hoja de cálculo automáticamente. El predeterminado es "Sheet".(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "(blank)" en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | Obtiene la cadena de visualización del valor de error de la celda |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | Obtiene el nombre del total general de la función. |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | Obtiene el texto dependiente de la configuración regional para el Nombre incorporado según el texto estándar proporcionado. |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | Obtiene el nombre de la función dependiente de la configuración regional según el nombre estándar de la función proporcionado. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "(Multiple Items)" en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "Grand Total" en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "Total" en la tabla dinámica. Necesita sobrescribir este método cuando la tabla dinámica contiene dos o más PivotFields en el área de datos.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) Obtiene el nombre de la protección en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) Obtiene el nombre de la etiqueta "Row Labels" en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | Obtiene el texto estándar del Nombre incorporado según el texto dependiente de la configuración regional proporcionado. |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | Obtiene el nombre estándar de la función según el nombre de función dependiente de la configuración regional proporcionado. |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | Obtiene el nombre de estilo de fuente estándar en inglés (Regular, Bold, Italic) para Encabezado/Pie de página según el nombre de estilo de fuente dependiente de la configuración regional proporcionado. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) Obtiene el nombre del tipo [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) en la tabla dinámica.(Heredado de [`GlobalizationSettings`](../globalizationsettings/).) |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | Obtiene el nombre del tipo de filas de tabla que consiste en todas las filas de la tabla referenciada. |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | Obtiene el nombre del tipo de filas de tabla que consiste en la fila actual de la tabla referenciada. |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | Obtiene el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada. El predeterminado es "Data", por lo que en la fórmula "#Data" representa la región de datos de la tabla. |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | Obtiene el nombre del tipo de filas de tabla que consiste en el encabezado de la tabla. El predeterminado es "Headers", por lo que en la fórmula "#Headers" representa el encabezado de la tabla. |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | Obtiene el nombre del tipo de filas de tabla que consiste en la fila total de la tabla referenciada. |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | Obtiene el nombre total de la función específica. |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | Establece el valor de cadena de visualización para el valor booleano de la celda |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | Establece el separador para los elementos en los datos de fila de la matriz en la fórmula. |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título de comentario. |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | Establece el nombre del total general de la función específica. |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | Establece el separador para la lista, los parámetros de la función, ...etc. |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | Establece el texto dependiente de la configuración regional para el nombre incorporado con el texto de nombre estándar proporcionado. |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | Establece el nombre de función dependiente de la configuración regional correspondiente al nombre de función estándar dado. |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | Establece el separador para las filas en los datos de la matriz en la fórmula. |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar dado. |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar dado. |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar dado. |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | Establece el nombre del tipo de filas de tabla que consiste en todas las filas de la tabla referenciada. |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | Establece el nombre del tipo de filas de tabla que consiste en la fila actual de la tabla referenciada. |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | Establece el nombre del tipo de filas de tabla que consiste en la región de datos de la tabla referenciada. |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | Establece el nombre del tipo de filas de tabla que consiste en el encabezado de la tabla. |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | Establece el nombre del tipo de filas de tabla que consiste en la fila total de la tabla referenciada. |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | Establece el nombre total de la función específica. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una instancia de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Establecer separador de lista personalizado
            settings.SetListSeparator(';');

            // Establecer cadenas de valores booleanos personalizadas
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Establecer nombres de funciones personalizados
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // Establecer nombres de tipo de fila de tabla personalizados
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // Establecer nombres de título de comentario personalizados
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // Se eliminó la línea Author ya que CommentTitleType no tiene ese valor de enumeración
            // Si necesitas establecer configuraciones relacionadas con el autor, deberías usar ThreadedCommentAuthor en su lugar

            // Aplicar la configuración de globalización al libro de trabajo
            workbook.Settings.GlobalizationSettings = settings;

            // Demostrar el uso en fórmulas
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // Guarda el libro de trabajo
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


