---
title: "Clase PivotField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotField. Representa un campo en un informe de tabla dinámica."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

Representa un campo en un informe de PivotTable.

```csharp
public class PivotField : IDisposable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllowDraggingToColumn](../../aspose.cells.pivot/pivotfield/allowdraggingtocolumn/) { get; set; } | Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es true. |
| [AllowDraggingToData](../../aspose.cells.pivot/pivotfield/allowdraggingtodata/) { get; set; } | Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es true. |
| [AllowDraggingToPage](../../aspose.cells.pivot/pivotfield/allowdraggingtopage/) { get; set; } | Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es true. |
| [AllowDraggingToRow](../../aspose.cells.pivot/pivotfield/allowdraggingtorow/) { get; set; } | Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es true. |
| [AllowRemovingFromView](../../aspose.cells.pivot/pivotfield/allowremovingfromview/) { get; set; } | Indica si este campo de tabla dinámica puede eliminarse de la vista de la tabla dinámica. El valor predeterminado es true. |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount/) { get; set; } | (**Obsolete.**) Representa el número de elementos superiores o inferiores que se muestran automáticamente en el campo de tabla dinámica especificado. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield/) { get; set; } | (**Obsolete.**) Representa el índice del campo de visualización automática. -1 significa el propio PivotField. Debe ser el índice de los campos de datos. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield/) { get; set; } | (**Obsolete.**) Representa el índice del campo que se ordena automáticamente. -1 significa el propio PivotField, otros indican la posición de los campos de datos. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex/) { get; set; } | Representa el índice en los campos de tabla dinámica de origen. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem/) { get; set; } | Obtiene o establece el elemento de página actualmente mostrado para este campo de tabla dinámica (solo campo de página). |
| [CurrentPageItemText](../../aspose.cells.pivot/pivotfield/currentpageitemtext/) { get; set; } | Obtiene el texto de visualización del elemento de página actual para este campo de tabla dinámica (solo campo de página). |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname/) { get; set; } | Representa el nombre de visualización del campo de tabla dinámica en la vista de tabla dinámica. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn/) { get; set; } | (**Obsolete.**) Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata/) { get; set; } | (**Obsolete.**) Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide/) { get; set; } | (**Obsolete.**) Indica si este campo de tabla dinámica puede eliminarse de la vista de tabla dinámica. El valor predeterminado es true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage/) { get; set; } | (**Obsolete.**) Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow/) { get; set; } | (**Obsolete.**) Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es true. |
| [Function](../../aspose.cells.pivot/pivotfield/function/) { get; set; } | Representa la función utilizada para resumir este campo de datos de tabla dinámica. |
| [GroupSettings](../../aspose.cells.pivot/pivotfield/groupsettings/) { get; } | Obtiene la configuración de grupo del campo de tabla dinámica. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow/) { get; set; } | Indica si se debe insertar una línea en blanco después de cada elemento. Solo para campos de fila. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow/) { get; set; } | (**Obsolete.**) Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort/) { get; set; } | (**Obsolete.**) Indica si los elementos de este campo de tabla dinámica se ordenan automáticamente en forma ascendente. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow/) { get; set; } | (**Obsolete.**) Indica si el campo de tabla dinámica especificado se muestra automáticamente. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort/) { get; set; } | (**Obsolete.**) Indica si los elementos de este campo de tabla dinámica se ordenan automáticamente. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals/) { get; set; } | Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield/) { get; } | Indica si este campo de tabla dinámica es un campo calculado. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/) { get; set; } | Indica si se deben incluir nuevos elementos al campo en el filtro manual. El valor predeterminado es false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/) { get; set; } | Indica si se deben insertar saltos de página después de cada elemento. El valor predeterminado es false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/) { get; set; } | Indica si se pueden seleccionar varios elementos en el campo de página. El valor predeterminado es false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels/) { get; set; } | Indica si se deben repetir las etiquetas del campo en la región de fila o columna. El valor predeterminado es false. |
| [IsValueFields](../../aspose.cells.pivot/pivotfield/isvaluefields/) { get; } | (**Obsolete.**) Indica si este campo representa campos de valores. |
| [IsValuesField](../../aspose.cells.pivot/pivotfield/isvaluesfield/) { get; } | Indica si este campo representa un campo de valores. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount/) { get; } | (**Obsolete.**) Obtiene el recuento de los elementos base en este pivot field. |
| [Items](../../aspose.cells.pivot/pivotfield/items/) { get; } | Obtenga todas las etiquetas de los elementos dinámicos en este campo. |
| [Name](../../aspose.cells.pivot/pivotfield/name/) { get; set; } | Representa el nombre de PivotField. |
| [NonAutoSortDefault](../../aspose.cells.pivot/pivotfield/nonautosortdefault/) { get; set; } | (**Obsolete.**) Indica si una operación de ordenación que se aplicará a este pivot field es una operación de autoordenación o una ordenación de datos simple. |
| [Number](../../aspose.cells.pivot/pivotfield/number/) { get; set; } | Representa el formato de visualización incorporado de números y fechas. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat/) { get; set; } | Representa el formato de visualización personalizado de números y fechas. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems/) { get; } | Obtenga los elementos base originales; |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems/) { get; } | Obtiene los elementos dinámicos del pivot field |
| [Position](../../aspose.cells.pivot/pivotfield/position/) { get; } | Representa el índice de `PivotField` en la región. |
| [RegionType](../../aspose.cells.pivot/pivotfield/regiontype/) { get; } | Especifica la región de la tabla dinámica donde se muestra este campo. |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems/) { get; set; } | Indica si se deben mostrar todos los elementos en la vista de PivotTable, incluso si no contienen datos resumidos. El valor predeterminado es false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact/) { get; set; } | (**Obsolete.**) Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de Pivot Table. Solo para campos de fila. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivotfield/showincompactform/) { get; set; } | Obtiene o establece un valor que indica si este campo de fila usa un diseño de forma compacta. Solo se aplica a campos de fila. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform/) { get; set; } | Obtiene o establece un valor que indica si este campo de fila usa un diseño de contorno. Solo se aplica a campos de fila. |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop/) { get; set; } | Indica si se deben mostrar los subtotales en la parte superior o inferior de los elementos. |
| [ShowValuesSetting](../../aspose.cells.pivot/pivotfield/showvaluessetting/) { get; } | Obtiene la configuración de mostrar valores cuando se está utilizando el cálculo ShowDataAs. |
| [SortSetting](../../aspose.cells.pivot/pivotfield/sortsetting/) { get; } | Obtiene todas las configuraciones de autoordenación |
| [Subtotals](../../aspose.cells.pivot/pivotfield/subtotals/) { get; set; } | Obtiene o establece los subtotales del campo. Solo para campos dinámicos de fila o columna. |
| [Top10AutoShowSettings](../../aspose.cells.pivot/pivotfield/top10autoshowsettings/) { get; } | Obtiene la configuración Top 10 AutoShow para un pivot field. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem/)(string, string) | Agrega un elemento de fórmula calculada al pivot field. |
| [ClearFilter](../../aspose.cells.pivot/pivotfield/clearfilter/)() | Borra la configuración de filtro en este pivot field. |
| [Dispose](../../aspose.cells.pivot/pivotfield/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [FilterByDate](../../aspose.cells.pivot/pivotfield/filterbydate/)(PivotFilterType, DateTime, DateTime) | Filtra por valores de fecha del campo dinámico de fila o columna. |
| [FilterByLabel](../../aspose.cells.pivot/pivotfield/filterbylabel/)(PivotFilterType, string, string) | Filtra por los títulos del campo pivot de fila o columna. |
| [FilterByValue](../../aspose.cells.pivot/pivotfield/filterbyvalue/)(int, PivotFilterType, double, double) | Filtra por los valores del campo pivot de datos. |
| [FilterTop10](../../aspose.cells.pivot/pivotfield/filtertop10/)(int, PivotFilterType, bool, int) | Filtra por los valores del campo pivot de datos. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula/)() | (**Obsolete.**) Obtiene la cadena de fórmula del campo calculado especificado. |
| [GetFilters](../../aspose.cells.pivot/pivotfield/getfilters/)() | Obtiene todos los filtros de tabla dinámica aplicados a este campo de tabla dinámica. |
| [GetFormula](../../aspose.cells.pivot/pivotfield/getformula/)() | Obtiene la fórmula del campo calculado. Solo funciona para el campo calculado. |
| [GetMaxValue](../../aspose.cells.pivot/pivotfield/getmaxvalue/)() | Obtiene el valor máximo de este campo. |
| [GetMinValue](../../aspose.cells.pivot/pivotfield/getminvalue/)() | Obtiene el valor máximo de este campo. |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype/)(PivotFilterType) | Obtiene el filtro de tabla dinámica del campo de tabla dinámica por tipo |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters/)() | (**Obsolete.**) Obtiene los filtros de tabla dinámica del campo de tabla dinámica |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals/)(PivotFieldSubtotalType) | Indica si se muestra el subtotal especificado para este campo de tabla dinámica. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group)() | Agrupa automáticamente el campo. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group_1)(PivotFieldGroupOptions) | Agrupa el campo de tabla dinámica con opciones. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby)(CustomPiovtFieldGroupItem[], bool) | (**Obsolete.**) Agrupa de forma personalizada el campo. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_1)(DiscreteGroupItem[], bool) | (**Obsolete.**) Agrupa de forma personalizada el campo. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_7)(double, bool) | (**Obsolete.**) Agrupa automáticamente el campo con intervalo |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_6)(PivotGroupByType[], double, bool) | (**Obsolete.**) Agrupa automáticamente el campo con interno |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_4)(double, double, double, bool) | (**Obsolete.**) Agrupa el archivo por número. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_5)(DateTime, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) Agrupa el archivo por los tipos de grupo de fecha. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_2)(bool, double, bool, double, double, bool) | (**Obsolete.**) Agrupa el archivo por número. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_3)(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) Agrupa el archivo por los tipos de grupo de fecha. |
| [HideAllDetails](../../aspose.cells.pivot/pivotfield/hidealldetails/)() | Oculta todos los detalles de cada elemento de tabla dinámica. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail/)(bool) | (**Obsolete.**) Establece si el detalle de todos los PivotItems en un campo de tabla dinámica está oculto. Es decir, colapsar/expandir este campo. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem)(int, bool) | (**Obsolete.**) Establece si el PivotItem específico en un campo de datos está oculto. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem_1)(string, bool) | (**Obsolete.**) Establece si el PivotItem específico en un campo de datos está oculto. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail/)(int, bool) | (**Obsolete.**) Establece si el detalle del PivotItem específico en un campo de tabla dinámica está oculto. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems/)() | (**Obsolete.**) Inicializa los elementos de tabla dinámica del campo de tabla dinámica |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem/)(int) | (**Obsolete.**) Indica si el PivotItem específico está oculto. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail/)(int) | (**Obsolete.**) Indica si se debe ocultar el detalle del PivotItem específico. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals/)(PivotFieldSubtotalType, bool) | Establece cómo subtotalizar el campo especificado. |
| [ShowAllDetails](../../aspose.cells.pivot/pivotfield/showalldetails/)() | Muestra todos los detalles de cada elemento de tabla dinámica. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_1)(PivotShowValuesAsType, int, int) | Establece el cálculo "Mostrar valores como" para este campo de tabla dinámica. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_2)(PivotShowValuesAsType, string, string) | Configura el cálculo "Mostrar valores como" para este campo de datos. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas)(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) | (**Obsolete.**) Muestra los valores del campo de datos en un formato de visualización diferente cuando se usa el cálculo ShowDataAs. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby)(SortOrder) | Ordena este campo dinámico. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_1)(SortOrder, int) | (**Obsolete.**) Ordena este campo dinámico. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_3)(SortOrder, int, string) | Ordena este campo dinámico. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_2)(SortOrder, int, PivotLineType, string) | (**Obsolete.**) Ordena este campo dinámico. |
| [Top10AutoShow](../../aspose.cells.pivot/pivotfield/top10autoshow/)(bool, bool, int, int) | Configura la configuración AutoShow Top10 para este campo dinámico. |
| [Ungroup](../../aspose.cells.pivot/pivotfield/ungroup/)() | Desagrupar el campo dinámico. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDemo
    {
        public static void PivotFieldExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar algunos datos a la hoja de cálculo
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Agregar una tabla dinámica a la hoja de cálculo
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "amount");

            // Establecer estilo de tabla pivot
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Acceder al campo de fila
            PivotField rowField = pivotTable.RowFields[0];

            // Establece propiedades del PivotField
            rowField.DisplayName = "Custom Display Name";
            rowField.IsAutoSubtotals = false;
            rowField.DragToColumn = true;
            rowField.DragToHide = true;
            rowField.DragToRow = true;
            rowField.DragToPage = true;
            rowField.DragToData = true;
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.IsRepeatItemLabels = true;
            rowField.IsIncludeNewItemsInFilter = true;
            rowField.IsInsertPageBreaksBetweenItems = true;
            rowField.ShowAllItems = true;
            rowField.NonAutoSortDefault = true;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;
            rowField.AutoSortField = -1;
            rowField.IsAutoShow = true;
            rowField.IsAscendShow = true;
            rowField.AutoShowCount = 5;
            rowField.AutoShowField = -1;
            rowField.Function = ConsolidationFunction.Sum;
            rowField.ShowValuesAs(PivotFieldDataDisplayFormat.PercentageOfTotal, 0, PivotItemPositionType.Next, 0);
            rowField.CurrentPageItem = 1;
            rowField.Number = 0;
            rowField.InsertBlankRow = true;
            rowField.ShowSubtotalAtTop = true;
            rowField.ShowInOutlineForm = true;
            rowField.NumberFormat = "0.00";
            rowField.ShowCompact = true;

            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


