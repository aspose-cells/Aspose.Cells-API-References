---
title: "Clase PivotTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotTable. Descripción resumida para PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Descripción resumida para PivotTable.

```csharp
public class PivotTable : IDisposable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllowMultipleFiltersPerField](../../aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/) { get; set; } | Especifica un valor booleano que indica si los campos de una PivotTable pueden tener varios filtros aplicados. |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription/) { get; set; } | Obtiene la descripción del texto alternativo. |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle/) { get; set; } | Obtiene y establece el título del texto alternativo. |
| [AutofitColumnWidthOnUpdate](../../aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/) { get; set; } | Indica si se debe ajustar automáticamente el ancho de columna al actualizar. |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype/) { get; set; } | Obtiene y establece el tipo de formato automático de la PivotTable. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields/) { get; } | Devuelve todos los campos base de pivote en la PivotTable. |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields/) { get; } | Devuelve un objeto PivotFields que se muestra actualmente como campos de columna. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand/) { get; set; } | (**Obsoleto.**) Indica si el informe de PivotTable muestra totales generales para las columnas. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption/) { get; set; } | Obtiene y establece el título personalizado del encabezado de columna de la PivotTable. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange/) { get; } | Devuelve un objeto CellArea que representa el rango que contiene el área de columna en el informe de PivotTable. Solo lectura. |
| [ConditionalFormats](../../aspose.cells.pivot/pivottable/conditionalformats/) { get; } | Obtiene los formatos condicionales de la tabla dinámica. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort/) { get; set; } | Indica si se debe considerar la lista personalizada incorporada al ordenar los datos. |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange/) { get; } | Devuelve un objeto [`CellArea`](../../aspose.cells/cellarea/) que representa el rango que contiene el área de datos en la lista entre la fila de encabezado y la fila de inserción. Solo lectura. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield/) { get; } | (**Obsoleto.**) Obtiene un objeto [`PivotField`](../pivotfield/) que representa todos los campos de datos en una PivotTable. Solo lectura. Solo se creará cuando haya dos o más campos de datos en la región de Datos. Por defecto está en la región de filas. Puedes arrastrarlo a la región de fila/columna con el método PivotTable.AddFieldToArea(). |
| [DataFieldHeaderName](../../aspose.cells.pivot/pivottable/datafieldheadername/) { get; set; } | Obtiene y establece el nombre del encabezado del campo del área de valores en la PivotTable. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields/) { get; } | Obtiene una [`PivotFieldCollection`](../pivotfieldcollection/) que representa todos los campos de datos en una PivotTable. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource/) { get; set; } | Obtiene y establece la fuente de datos de la tabla dinámica. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring/) { get; set; } | Indica si el informe de PivotTable muestra una cadena personalizada en las celdas que contienen errores. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems/) { get; set; } | Indica si los elementos en las áreas de fila y columna son visibles cuando el área de datos de la PivotTable está vacía. El valor predeterminado es verdadero. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring/) { get; set; } | Indica si el informe de PivotTable muestra una cadena personalizada si el valor es nulo. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting/) { get; set; } | Especifica un valor booleano que indica si se permite al usuario editar las celdas en el área de datos de la pivottable. El valor predeterminado es falso. |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown/) { get; set; } | Indica si la perforación está habilitada. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog/) { get; set; } | Indica si el cuadro de diálogo del campo de PivotTable está disponible cuando el usuario hace doble clic en el campo de PivotTable. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist/) { get; set; } | Indica si la lista de campos de la PivotTable está disponible en la vista de Excel. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard/) { get; set; } | Indica si el asistente de PivotTable está disponible. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring/) { get; set; } | Obtiene la cadena que se muestra en celdas que contienen errores cuando la propiedad DisplayErrorString es verdadera. El valor predeterminado es una cadena vacía. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource/) { get; } | (**Obsolete.**) Obtiene la fuente de datos de conexión externa. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending/) { get; set; } | Indica si los campos en la PivotTable están ordenados en un orden no predeterminado en la lista de campos. |
| [FilterArea](../../aspose.cells.pivot/pivottable/filterarea/) { get; } | Obtiene el área de la región de filtro. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname/) { get; set; } | Devuelve la etiqueta que se muestra en el encabezado de la columna o fila de total general. El valor predeterminado es la cadena "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows/) { get; set; } | (**Obsolete.**) Indica si se deben agregar filas en blanco. Esta propiedad solo se aplica a los tipos de formato automático de PivotTable que requieren agregar filas en blanco. |
| [Indent](../../aspose.cells.pivot/pivottable/indent/) { get; set; } | Especifica el incremento de sangría para el eje compacto y puede usarse para establecer el diseño del informe en forma compacta. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat/) { get; set; } | Indica si el informe de PivotTable se formatea automáticamente. Casilla de verificación "autoformat table" que está en la opción de PivotTable para Excel 2003. |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible/) { get; set; } | Especifica si la PivotTable es compatible con Excel2003 al actualizar la PivotTable; si es verdadero, una cadena debe tener 255 caracteres o menos, por lo que si la cadena supera los 255 caracteres, se truncará. Si es falso, una cadena no tendrá la restricción mencionada. El valor predeterminado es verdadero. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones/) { get; set; } | Indica si el informe de PivotTable muestra el diseño clásico de tabla dinámica. (permite arrastrar campos en la cuadrícula) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters/) { get; set; } | (**Obsolete.**) Especifica un valor booleano que indica si los campos de una PivotTable pueden tener varios filtros aplicados. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected/) { get; set; } | Indica si esta PivotTable está seleccionada. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles/) { get; set; } | (**Obsolete.**) Indica si los nombres de PivotItem deben repetirse en la parte superior de cada página impresa. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate/) { get; set; } | Indica si el informe de PivotTable se recalcula solo a petición del usuario. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels/) { get; set; } | Obtiene o establece si se deben combinar las etiquetas de campos de fila/columna que abarcan varias celdas. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit/) { get; set; } | (**Obsolete.**) Especifica un valor booleano que indica si los campos de una PivotTable pueden tener varios filtros aplicados. |
| [Name](../../aspose.cells.pivot/pivottable/name/) { get; set; } | Obtiene el nombre de la PivotTable |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring/) { get; set; } | Obtiene la cadena que se muestra en celdas que contienen valores nulos cuando la propiedad DisplayNullString es verdadera. El valor predeterminado es una cadena vacía. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder/) { get; set; } | Obtiene y establece el orden en que los campos de página se añaden al diseño del informe de PivotTable. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields/) { get; } | Devuelve una [`PivotFieldCollection`](../pivotfieldcollection/) que se muestra actualmente como campos de página. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount/) { get; set; } | Obtiene el número de campos de página en cada columna o fila del informe de PivotTable. |
| [PivotCache](../../aspose.cells.pivot/pivottable/pivotcache/) { get; } | Obtiene la fuente de datos. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters/) { get; } | Devuelve todos los filtros en la tabla dinámica. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions/) { get; } | (**Obsolete.**) Obtiene las condiciones de formato de la tabla dinámica. |
| [PivotFormats](../../aspose.cells.pivot/pivottable/pivotformats/) { get; } | Obtiene todos los formatos de celda aplicados a esta tabla dinámica. |
| [PivotTableStyle](../../aspose.cells.pivot/pivottable/pivottablestyle/) { get; set; } | Obtiene la configuración de TableStyle de esta tabla dinámica. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename/) { get; set; } | Obtiene o establece el nombre del estilo de la tabla dinámica. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype/) { get; set; } | Obtiene y establece el estilo incorporado de la tabla dinámica. |
| [PreserveCellFormattingOnUpdate](../../aspose.cells.pivot/pivottable/preservecellformattingonupdate/) { get; set; } | Indica si se debe preservar el formato de celda ([`PivotTableFormat`](../pivottableformat/)) cuando la tabla dinámica se actualiza o recalcula. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting/) { get; set; } | (**Obsolete.**) Indica si el formato de celda ([`PivotTableFormat`](../pivottableformat/)) se conserva cuando la tabla dinámica se actualiza o recalcula. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill/) { get; set; } | Especifica un valor booleano que indica si los indicadores de desglose deben imprimirse. Imprime los botones de expandir/contraer cuando se muestra en la tabla dinámica. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles/) { get; set; } | Indica si los títulos de impresión para la hoja de cálculo se establecen en función del informe de la tabla dinámica. El valor predeterminado es false. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile/) { get; set; } | Indica si se actualizan los datos al abrir el archivo. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate/) { get; } | Obtiene la fecha y hora de la última actualización de la tabla dinámica. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho/) { get; } | Obtiene el nombre del último usuario que actualizó esta tabla dinámica |
| [RepeatItemsOnEachPrintedPage](../../aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/) { get; set; } | Indica si los títulos del elemento de tabla dinámica en el área de filas se repiten en cada página impresa para los campos de tabla dinámica en forma tabular. |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields/) { get; } | Devuelve una [`PivotFieldCollection`](../pivotfieldcollection/) que se muestran actualmente como campos de fila. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand/) { get; set; } | (**Obsolete.**) Indica si se deben mostrar los totales generales para las filas de esta tabla dinámica. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption/) { get; set; } | Obtiene y establece el título personalizado del encabezado de fila en esta tabla dinámica. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange/) { get; } | Devuelve un objeto CellArea que representa el rango que contiene el área de filas en el informe de la tabla dinámica. Solo lectura. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata/) { get; set; } | Indica si los datos del informe de la tabla dinámica se guardan con el libro de trabajo. |
| [ShowColumnGrandTotals](../../aspose.cells.pivot/pivottable/showcolumngrandtotals/) { get; set; } | Indica si se deben mostrar los totales generales para las columnas de esta tabla dinámica. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips/) { get; set; } | Indica si se deben mostrar descripciones emergentes para las celdas de datos de la tabla dinámica. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill/) { get; set; } | Obtiene y establece si se muestran los botones de expandir/contraer. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol/) { get; set; } | Indica si se deben incluir columnas vacías en la tabla |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow/) { get; set; } | Indica si se deben incluir filas vacías en la tabla. |
| [ShowHeaders](../../aspose.cells.pivot/pivottable/showheaders/) { get; set; } | Indica si se deben mostrar los títulos de los campos de datos y los títulos de los campos de tabla dinámica en el eje de filas y en el eje de columnas en la vista de la tabla dinámica. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips/) { get; set; } | Especifica un valor booleano que indica si la información de propiedades de los miembros debe omitirse de las descripciones emergentes de la tabla dinámica. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader/) { get; set; } | Indica si el encabezado de columna en la tabla dinámica debe tener el estilo aplicado. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/) { get; set; } | Indica si se aplica formato de rayas para la columna. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn/) { get; set; } | Indica si se aplica el formato de columna. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader/) { get; set; } | Indica si el encabezado de fila en la tabla dinámica debe tener el estilo aplicado. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes/) { get; set; } | Indica si se aplica formato de rayas en filas. |
| [ShowRowGrandTotals](../../aspose.cells.pivot/pivottable/showrowgrandtotals/) { get; set; } | Indica si se deben mostrar los totales generales para las filas de la tabla dinámica. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption/) { get; set; } | (**Obsolete.**) Indica si el título del encabezado de fila se muestra en el informe de la tabla dinámica Indica si se muestran los títulos de los campos y los menús desplegables de filtro |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow/) { get; set; } | Indica si se muestra la fila de valores. |
| [SourceType](../../aspose.cells.pivot/pivottable/sourcetype/) { get; } | Obtiene el tipo de origen de datos de la tabla dinámica. |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems/) { get; set; } | Indica si los elementos de campo de página ocultos en el informe de la tabla dinámica se incluyen en los subtotales de fila y columna, totales de bloque y totales generales. El valor predeterminado es False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1/) { get; } | Devuelve un objeto CellArea que representa el rango que contiene todo el informe de la tabla dinámica, pero no incluye los campos de página. Solo lectura. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2/) { get; } | Devuelve un objeto CellArea que representa el rango que contiene todo el informe de la tabla dinámica, incluye los campos de página. Solo lectura. |
| [Tag](../../aspose.cells.pivot/pivottable/tag/) { get; set; } | Obtiene y establece una cadena definida por el usuario que está asociada a esta vista de tabla dinámica. |
| [TopRightArea](../../aspose.cells.pivot/pivottable/toprightarea/) { get; } | Representa el área en blanco en la esquina superior derecha de la tabla dinámica (esquina superior izquierda para hojas RTL). |
| [ValuesField](../../aspose.cells.pivot/pivottable/valuesfield/) { get; } | Obtiene un objeto [`PivotField`](../pivotfield/) que representa todos los campos de datos en una tabla dinámica. Solo lectura. Solo se creará cuando haya dos o más campos de datos en la región de Datos. Por defecto está en la región de filas. Puedes arrastrarlo a la región de fila/columna con el método PivotTable.AddFieldToArea(). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield)(string, string) | Agrega un campo calculado al campo dinámico y lo arrastra al área de datos. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield_1)(string, string, bool) | Agrega un campo calculado al campo dinámico. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_1)(PivotFieldType, int) | Agrega el campo al área específica. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea)(PivotFieldType, PivotField) | Agrega el campo al área específica. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_2)(PivotFieldType, string) | Agrega el campo al área específica. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata_1)() | Calcula los datos de la tabla dinámica en celdas. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata)(PivotTableCalculateOption) | Calcula la tabla dinámica con opciones. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange/)() | Calcula el rango de la tabla dinámica. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource/)(string[]) | Cambia el origen de datos de la tabla dinámica. |
| [ClearAll](../../aspose.cells.pivot/pivottable/clearall/)() | Elimina todos los campos de las regiones. |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata/)() | Borra los datos y el formato de la vista de tabla dinámica. |
| [ClearFilters](../../aspose.cells.pivot/pivottable/clearfilters/)() | Elimina todos los filtros de esta tabla dinámica. |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle/)(PivotTable) | Copia el estilo con nombre de otra tabla dinámica. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [ExportViewToJson](../../aspose.cells.pivot/pivottable/exportviewtojson/)(PivotViewToJsonOptions) | Exporta la vista de tabla dinámica como JSON. |
| [Fields](../../aspose.cells.pivot/pivottable/fields/)(PivotFieldType) | (**Obsolete.**) Obtiene los campos específicos por el tipo de campo. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format)(CellArea, Style) | Da formato al área seleccionada de la tabla dinámica. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_1)(PivotArea, Style) | Da formato al área seleccionada de la tabla dinámica. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_2)(int, int, Style) | Da formato a la celda en el área de la tabla dinámica |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall/)(Style) | Da formato a todas las celdas en el área de la tabla dinámica |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow/)(int, Style) | Da formato a los datos de fila en el área de la tabla dinámica |
| [GetButtonArea](../../aspose.cells.pivot/pivottable/getbuttonarea/)(PivotFieldType) | Obtiene el área que contiene el botón de campo. |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname/)(string) | Obtiene el objeto [`Cell`](../../aspose.cells/cell/) por el nombre para mostrar del PivotField. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren/)() | (**Obsolete.**) Obtiene las tablas dinámicas hijas que usan estos datos de tabla dinámica como fuente de datos. |
| [GetDependentPivotTables](../../aspose.cells.pivot/pivottable/getdependentpivottables/)() | Obtiene todas las `PivotTable`s que usan esta tabla dinámica como su fuente de datos. |
| [GetFields](../../aspose.cells.pivot/pivottable/getfields/)(PivotFieldType) | Obtiene la lista específica de campos de tabla dinámica por la región. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks/)() | (**Obsolete.**) Obtiene la lista de índices de fila de la tabla dinámica de saltos de página horizontales |
| [GetHorizontalPageBreaks](../../aspose.cells.pivot/pivottable/gethorizontalpagebreaks/)() | Obtiene los saltos de página horizontales de esta tabla dinámica. |
| [GetNamesOfSourceDataConnections](../../aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/)() | Obtiene los nombres de las conexiones de datos de origen externo. |
| [GetPivotTablesWithSamePivotCache](../../aspose.cells.pivot/pivottable/getpivottableswithsamepivotcache/)() | Obtiene todas las tablas dinámicas con la misma caché de tabla dinámica. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource)() | Obtén la fuente de datos de esta tabla dinámica. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource_1)(bool) | Obtén la fuente de datos de esta tabla dinámica. |
| [GetSourceDataConnections](../../aspose.cells.pivot/pivottable/getsourcedataconnections/)() | Obtiene las fuentes de datos de conexión externa. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move_1)(string) | (**Obsolete.**) Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move)(int, int) | (**Obsolete.**) Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [MoveItem](../../aspose.cells.pivot/pivottable/moveitem/)(PivotFieldType, string[], bool, int) | Mueve un elemento hacia arriba o abajo. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_2)(string) | Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto)(int, int) | Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_1)(int, int, int) | Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh)() | Actualiza [`PivotCache`](./pivotcache/) desde la fuente de datos y calcula los datos y el estilo para la vista de tabla dinámica. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh_1)(PivotTableRefreshOption) | Actualiza [`PivotCache`](./pivotcache/) desde la fuente de datos y calcula los datos y el estilo para la vista de tabla dinámica. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata)() | (**Obsolete.**) Actualiza los datos desde su fuente de datos a la caché de tabla dinámica. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata_1)(PivotTableRefreshOption) | (**Obsolete.**) Actualiza los datos y la configuración de la tabla dinámica desde su fuente de datos con opciones. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_1)(PivotFieldType, int) | Elimina un campo de una región de tabla dinámica específica. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield)(PivotFieldType, PivotField) | Eliminar campo del área de campo específica |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_2)(PivotFieldType, string) | Elimina un campo de un área de campo específica |
| [SelectArea](../../aspose.cells.pivot/pivottable/selectarea/)(CellArea) | Selecciona un área de la vista de tabla dinámica. |
| [ShowDetail](../../aspose.cells.pivot/pivottable/showdetail/)(int, int, bool, int, int) | Muestra el detalle de un elemento en la región de datos en una tabla nueva. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform/)() | Diseña la vista de la tabla dinámica en forma compacta. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform/)() | Diseña la tabla dinámica en forma de esquema. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform/)() | Diseña la tabla dinámica en forma tabular. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage/)(PivotField) | Muestra todas las páginas de filtro de informe según el PivotField, el PivotField debe estar ubicado en los PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex/)(int) | Muestra todas las páginas de filtro de informe según el índice de posición en los PageFields. |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname/)(string) | Muestra todas las páginas de filtro de informe según el nombre del PivotField, el PivotField debe estar ubicado en los PageFields. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotTableDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Establecer datos de muestra
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Crear tabla dinámica
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];

            // Agregar campos
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Estilizar la tabla dinámica
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Personalizar el campo de fila
            PivotField rowField = pivot.RowFields[0];
            rowField.DisplayName = "Fruit Category";

            // Actualizar y calcular datos
            pivot.RefreshData();
            pivot.CalculateData();

            // Guarda el libro de trabajo
            book.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


