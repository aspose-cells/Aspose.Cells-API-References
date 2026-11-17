---
title: "Clase PivotField"
linktitle: "PivotField"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "PivotField class. Encapsula el objeto que representa pivotfield en Go."
type: docs
weight: 200
url: /es/go-cpp/pivotfield/
---

## PivotField class

Represents a field in a PivotTable report.

```go

type PivotField struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetPivotItems](./getpivotitems/) | Obtiene los elementos pivot del campo pivot |
| [GetMaxValue](./getmaxvalue/) | Obtiene el valor máximo de este campo. |
| [GetMinValue](./getminvalue/) | Obtiene el valor máximo de este campo. |
| [GetGroupSettings](./getgroupsettings/) | Obtiene la configuración de grupo del campo pivot. |
| [InitPivotItems](./initpivotitems/) | Inicializa los elementos pivot del campo pivot |
| [Group](./group/) | Agrupa automáticamente el campo. |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | Agrupa el campo pivot con opciones. |
| [GroupBy](./groupby/) | Agrupa el campo de forma personalizada. |
| [Ungroup](./ungroup/) | Desagrupa el campo pivot. |
| [GetPivotFilterByType](./getpivotfilterbytype/) | Obtiene el filtro de pivote del campo de pivote por tipo |
| [GetFilters](./getfilters/) | Obtiene todos los filtros de pivote aplicados a este campo de pivote. |
| [ClearFilter](./clearfilter/) | Borra la configuración del filtro en este campo de pivote. |
| [FilterTop10](./filtertop10/) | Filtra por valores del campo pivot de datos. |
| [FilterByValue](./filterbyvalue/) | Filtra por valores del campo pivot de datos. |
| [FilterByLabel](./filterbylabel/) | Filtra por leyendas de la fila o columna del campo pivot. |
| [FilterByDate](./filterbydate/) | Filtra por valores de fecha del campo de pivote de fila o columna. |
| [IsCalculatedField](./iscalculatedfield/) | Indica si este campo de pivote es un campo calculado. |
| [GetFormula](./getformula/) | Obtiene la fórmula del campo calculado. Solo funciona para campos calculados. |
| [IsValuesField](./isvaluesfield/) | Indica si este campo representa el campo de valores. |
| [GetBaseIndex](./getbaseindex/) | Representa el índice en los campos de pivote de origen. |
| [SetBaseIndex](./setbaseindex/) | Representa el índice en los campos de pivote de origen. |
| [GetPosition](./getposition/) | Representa el índice del PivotField en la región. |
| [GetRegionType](./getregiontype/) | Especifica la región de la tabla dinámica donde se muestra este campo. |
| [GetName](./getname/) | Representa el nombre del PivotField. |
| [SetName](./setname/) | Representa el nombre del PivotField. |
| [GetDisplayName](./getdisplayname/) | Representa el nombre visible del campo de pivote en la vista de la tabla dinámica. |
| [SetDisplayName](./setdisplayname/) | Representa el nombre visible del campo de pivote en la vista de la tabla dinámica. |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | Establece cómo subtotalizar el campo especificado. |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | Indica si se muestra el subtotal especificado para este campo de pivote. |
| [GetSubtotals](./getsubtotals/) | Obtiene o establece los subtotales del campo. Solo para campos de pivote de fila o columna. |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | Obtiene o establece los subtotales del campo. Solo para campos de pivote de fila o columna. |
| [IsAutoSubtotals](./isautosubtotals/) | Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es verdadero. |
| [SetIsAutoSubtotals](./setisautosubtotals/) | Indica si el campo especificado muestra subtotales automáticos. El valor predeterminado es verdadero. |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es verdadero. |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | Indica si el campo especificado puede arrastrarse a la región de filas. El valor predeterminado es verdadero. |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es verdadero. |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | Indica si el campo especificado puede arrastrarse a la región de columnas. El valor predeterminado es verdadero. |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es verdadero. |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | Indica si el campo especificado puede arrastrarse a la región de página. El valor predeterminado es verdadero. |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | Indica si este campo de pivote puede eliminarse de la vista de la tabla dinámica. El valor predeterminado es verdadero. |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | Indica si este campo de pivote puede eliminarse de la vista de la tabla dinámica. El valor predeterminado es verdadero. |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es verdadero. |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | Indica si el campo especificado puede arrastrarse a la región de valores. El valor predeterminado es verdadero. |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | Indica si se pueden seleccionar varios elementos en el campo de página. El valor predeterminado es falso. |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | Indica si se pueden seleccionar varios elementos en el campo de página. El valor predeterminado es falso. |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | Indica si se repiten las etiquetas del campo en la región. El valor predeterminado es falso. |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Indica si se repiten las etiquetas del campo en la región. El valor predeterminado es falso. |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Indica si se incluyen nuevos elementos al campo en el filtro manual. El valor predeterminado es falso. |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Indica si se incluyen nuevos elementos al campo en el filtro manual. El valor predeterminado es falso. |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Indica si se insertan saltos de página después de cada elemento. El valor predeterminado es falso. |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Indica si se insertan saltos de página después de cada elemento. El valor predeterminado es falso. |
| [GetShowAllItems](./getshowallitems/) | Indica si se deben mostrar todos los elementos en la vista de la tabla dinámica, incluso si no contienen datos resumidos. El valor predeterminado es false. |
| [SetShowAllItems](./setshowallitems/) | Indica si se deben mostrar todos los elementos en la vista de la tabla dinámica, incluso si no contienen datos resumidos. El valor predeterminado es false. |
| [SortBy_SortOrder](./sortby_sortorder/) | Ordena este campo dinámico. |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | Ordena este campo dinámico. |
| [GetSortSetting](./getsortsetting/) | Obtiene todas las configuraciones de ordenación automática |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | Obtiene la configuración Top 10 AutoShow para un campo dinámico. |
| [Top10AutoShow](./top10autoshow/) | Configura la configuración Top10 AutoShow para este campo dinámico. |
| [GetFunction](./getfunction/) | Representa la función utilizada para resumir este campo de datos de la tabla dinámica. |
| [SetFunction](./setfunction/) | Representa la función utilizada para resumir este campo de datos de la tabla dinámica. |
| [ShowValuesAs](./showvaluesas/) | Muestra los valores del campo de datos con un formato de visualización diferente cuando se utiliza el cálculo ShowDataAs. |
| [GetShowValuesSetting](./getshowvaluessetting/) | Obtiene la configuración de visualización de valores cuando se utiliza el cálculo ShowDataAs. |
| [GetCurrentPageItem](./getcurrentpageitem/) | Representa el elemento de página seleccionado actualmente del campo de página para filtrar datos. Solo válido para campos de página. |
| [SetCurrentPageItem](./setcurrentpageitem/) | Representa el elemento de página seleccionado actualmente del campo de página para filtrar datos. Solo válido para campos de página. |
| [GetInsertBlankRow](./getinsertblankrow/) | Indica si se debe insertar una línea en blanco después de cada elemento. Solo para campos de fila. |
| [SetInsertBlankRow](./setinsertblankrow/) | Indica si se debe insertar una línea en blanco después de cada elemento. Solo para campos de fila. |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | Indica si se deben mostrar subtotales en la parte superior o inferior de los elementos cuando ShowInOutlineForm es verdadero, entonces |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | Indica si se deben mostrar subtotales en la parte superior o inferior de los elementos cuando ShowInOutlineForm es verdadero, entonces |
| [GetShowInOutlineForm](./getshowinoutlineform/) | Indica si se debe organizar este campo en forma de esquema en la vista de la tabla dinámica. |
| [SetShowInOutlineForm](./setshowinoutlineform/) | Indica si se debe organizar este campo en forma de esquema en la vista de la tabla dinámica. |
| [GetNumber](./getnumber/) | Representa el formato de visualización incorporado de números y fechas. |
| [SetNumber](./setnumber/) | Representa el formato de visualización incorporado de números y fechas. |
| [Get_NumberFormat](./get_numberformat/) | Representa el formato de visualización personalizado de números y fechas. |
| [SetNumberFormat](./setnumberformat/) | Representa el formato de visualización personalizado de números y fechas. |
| [HideAllDetails](./hidealldetails/) | Oculta todos los detalles |
| [ShowAllDetails](./showalldetails/) | Mostrar todos los detalles |
| [GetItems](./getitems/) | Obtiene todas las etiquetas de los elementos dinámicos en este campo. |
| [GetOriginalItems](./getoriginalitems/) | Obtiene los elementos base originales; |
| [AddCalculatedItem](./addcalculateditem/) | Agrega un elemento de fórmula calculada al campo dinámico. |
| [GetShowCompact](./getshowcompact/) | Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de la tabla dinámica |
| [SetShowCompact](./setshowcompact/) | Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de la tabla dinámica |
