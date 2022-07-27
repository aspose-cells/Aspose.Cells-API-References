---
title: PivotTable
second_title: Referencia de API de Aspose.Cells para .NET
description: Descripción resumida de la tabla dinámica.
type: docs
weight: 4690
url: /es/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Descripción resumida de la tabla dinámica.

```csharp
public class PivotTable : IDisposable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | Obtiene la descripción del texto alternativo |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | Obtiene el título del altertext |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | Obtiene el tipo de formato automático de tabla dinámica. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | Devuelve un objeto PivotFields que incluye todos los campos en el informe de tabla dinámica |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | Devuelve un objeto PivotFields que actualmente se muestra como campos de columna. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | Indica si el informe de tabla dinámica muestra los totales generales de las columnas. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | Obtiene el título del encabezado de columna de la tabla dinámica. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | Devuelve un objeto CellArea que representa el rango que contiene el área de la columna en el informe de tabla dinámica. Solo lectura. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | Indica si se debe considerar una lista personalizada integrada al ordenar data |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | Devuelve un objeto CellArea que representa el rango que contiene los datos area en la lista entre la fila de encabezado y la fila de inserción. Solo lectura. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | Obtiene un objeto PivotField que representa todos los campos de datos en una tabla dinámica. Solo lectura. Sería inicial solo cuando hay dos o más campos de datos en DataPiovtFiels. Solo se usa para agregar DataPivotField a la fila/columna de la tabla dinámica. área . El valor predeterminado está en el área de la fila. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | Obtiene un objeto PivotField que representa todos los campos de datos en una tabla dinámica. Solo lectura. Sería inicial solo cuando hay dos o más campos de datos en DataPiovtFiels. Solo se usa para agregar DataPivotField a la fila/columna de la tabla dinámica. área . El valor predeterminado está en el área de la fila. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | Obtiene y establece la fuente de datos de la tabla dinámica. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | Indica si el informe de tabla dinámica muestra una cadena personalizada en las celdas que contienen errores. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | Indica si los elementos de las áreas de fila y columna están visibles cuando el área de datos de la tabla dinámica está vacía. El valor predeterminado es verdadero. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | Indica si el informe de tabla dinámica muestra una cadena personalizada en las celdas que contienen valores nulos. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | Especifica un valor booleano que indica si el usuario puede editar las celdas en el área de datos de la tabla dinámica. Habilitar la edición de celdas en el área de valores |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | Obtiene si el desglose está habilitado. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | Indica si el cuadro de diálogo Campo de tabla dinámica está disponible cuando el usuario hace doble clic en el campo de tabla dinámica. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | Obtiene si habilita la lista de campos para la tabla dinámica. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | Indica si el Asistente para tablas dinámicas está disponible. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | Obtiene la cadena que se muestra en las celdas que contienen errores cuando la propiedad DisplayErrorString es verdadera. El valor predeterminado es una cadena vacía. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | Obtiene la fuente de datos de la conexión externa. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | Especifica un valor booleano que indica si los campos de la tabla dinámica están ordenados en un orden diferente al predeterminado en la lista de campos. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | Devuelve la etiqueta de cadena de texto que se muestra en el encabezado de fila o columna de total general. El valor predeterminado es la cadena "Total general". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | Indica si se deben agregar filas en blanco. Esta propiedad solo se aplica a los tipos de formato automático de tabla dinámica que necesitan agregar filas en blanco. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | Especifica el incremento de sangría para el eje compacto y se puede usar para establecer el Diseño del informe en Forma compacta. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | Indica si el informe de tabla dinámica se formatea automáticamente. Casilla de verificación "tabla de formato automático" que se encuentra en la opción pivotable para Excel 2003 Casilla de verificación "ajustar automáticamente el ancho de columna al actualizar" que se encuentra en la tabla dinámica Opciones: formato de diseño para Excel 2007 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | Especifica si la tabla dinámica es compatible con Excel 2003 al actualizar la tabla dinámica, si es verdadero, una cadena debe tener 255 caracteres o menos, por lo que si la cadena tiene más de 255 caracteres, se truncará. si es falso, una cadena no tendrá la restricción mencionada anteriormente. El valor predeterminado es verdadero. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | Indica si el informe de tabla dinámica muestra el diseño clásico de tabla dinámica. (permite arrastrar campos en la cuadrícula) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros establecidos. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | Indica si la tabla dinámica está seleccionada. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | Un bit que especifica si los títulos de los elementos pivote en el eje de fila se repiten en cada página impresa para los campos pivote en formato tabular. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | Indica si el informe de tabla dinámica se recalcula solo a pedido del usuario. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | Indica si las etiquetas de elemento de fila exterior, elemento de columna, subtotal, y total general del informe de tabla dinámica especificado utilizan celdas combinadas. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros establecidos. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | Obtiene el nombre de la tabla dinámica |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | Obtiene la cadena que se muestra en las celdas que contienen valores nulos cuando la propiedad DisplayNullString es verdadera. El valor predeterminado es una cadena vacía. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | Obtiene el orden en que se agregan los campos de página al diseño del informe de tabla dinámica. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | Devuelve un objeto PivotFields que actualmente se muestra como campos de página. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | Obtiene el número de campos de página en cada columna o fila del informe de tabla dinámica. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | Devuelve un objeto PivotFilterCollection. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | Obtiene las Condiciones de formato de la tabla dinámica. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | Obtiene y establece el nombre del estilo pivotable. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | Obtiene y establece el estilo de tabla dinámica integrado. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | Indica si se conserva el formato cuando se actualiza o se vuelve a calcular la tabla dinámica. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | Especifica un valor booleano que indica si se deben imprimir los indicadores de exploración. imprime los botones de expandir/contraer cuando se muestran en la tabla dinámica. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | Indica si los títulos de impresión para la hoja de cálculo se establecen en base en el informe de tabla dinámica. El valor predeterminado es falso. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | Indica si Actualizar Datos o no. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | Indica si Actualizar datos al abrir archivo. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | Obtiene la fecha en que se actualizó por última vez la tabla dinámica. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | Obtiene el nombre del usuario que actualizó por última vez la tabla dinámica |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | Devuelve un objeto PivotFields que actualmente se muestra como campos de fila. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | Indica si el informe de tabla dinámica muestra los totales generales de las filas. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | Obtiene el título del encabezado de fila de la tabla dinámica. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | Devuelve un objeto CellArea que representa el rango que contiene el área de fila en el informe de tabla dinámica. Solo lectura. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | Indica si los datos del informe de tabla dinámica se guardan con el libro de trabajo. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | Especifica un valor booleano que indica si se debe mostrar información sobre herramientas para las celdas de datos de la tabla dinámica. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | Obtiene si se muestran los botones expandir/contraer. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | Especifica un valor booleano que indica si incluir columnas vacías en la tabla |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | Especifica un valor booleano que indica si se deben incluir filas vacías en la tabla. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | Especifica un valor booleano que indica si la información de propiedad de miembro se debe omitir de la información sobre herramientas de la tabla dinámica. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | Indica si el encabezado de la columna en la tabla dinámica debe tener el estilo aplicado. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | Indica si se aplica el formato de franja de columna. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | Indica si se aplica el formato de franja de columna. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | Indica si el encabezado de la fila en la tabla dinámica debe tener el estilo aplicado. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | Indica si se aplica el formato de franja de fila. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | Indica si el título de encabezado de fila se muestra en el informe de tabla dinámica Indica si Mostrar títulos de campo y filtros desplegables |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | Especifica un valor booleano que indica si mostrar valores fila. mostrar los valores fila |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | Indica si los elementos de campo de página ocultos en el informe de tabla dinámica se incluyen en subtotales de fila y columna, totales de bloque y totales generales. El valor predeterminado es Falso. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | Devuelve un objeto CellArea que representa el rango que contiene todo el informe de tabla dinámica, pero no incluye campos de página. Solo lectura. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | Devuelve un objeto CellArea que representa el rango que contiene todo el informe de tabla dinámica, incluye campos de página. Solo lectura. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | Obtiene una cadena guardada con el informe de tabla dinámica. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | Agrega un campo calculado al campo pivote y lo arrastra al área de datos. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | Agrega un campo calculado al campo pivote. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | Agrega el campo al área específica. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | Agrega el campo al área específica. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | Agrega el campo al área específica. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | Calcula los datos de la tabla dinámica en celdas. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | Calcula el rango de la tabla dinámica. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | Establecer los datos de origen de la tabla dinámica. Hoja1!$A$1:$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | Borrar datos y formato de tabla dinámica |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | Copia el estilo con nombre de otra tabla dinámica. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | Realiza tareas definidas por la aplicación asociadas con la liberación, liberación o restablecimiento de recursos no administrados. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | Obtiene los campos específicos por tipo de campo. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | Formatea la celda en el área pivotable |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | Formatea todas las celdas en el área pivotable |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | Dar formato a los datos de la fila en el área pivotable |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | Obtiene el objeto Cell por el DisplayName de PivotField |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | Obtiene las tablas dinámicas secundarias que usan estos datos de tabla dinámica como origen de datos. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | obtener la lista de índice de filas de tabla dinámica de saltos de página horizontales |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | Obtener los datos de origen de la tabla dinámica. |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | Mueve la tabla dinámica a una ubicación diferente en la hoja de trabajo. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | Mueve la tabla dinámica a una ubicación diferente en la hoja de trabajo. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | Actualiza los datos y la configuración de la tabla dinámica desde su origen de datos. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | Elimina un campo de un campo específico area |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | Eliminar campo de campo específico area |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | Elimina un campo de un campo específico area |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | Establece el grupo de campo automático por la tabla dinámica. |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | Establece el grupo de campo automático por la tabla dinámica. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | Establece el grupo de campo manual por la tabla dinámica. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | Establece el grupo de campo manual por la tabla dinámica. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | Establece el grupo de campo manual por la tabla dinámica. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | Establece el grupo de campo manual por la tabla dinámica. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | Conjuntos desagrupados por la tabla dinámica |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | Conjuntos desagrupados por la tabla dinámica |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | Diseña la tabla dinámica en formato compacto. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | Diseña la tabla dinámica en forma de esquema. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | Presenta la tabla dinámica en formato tabular. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | Mostrar todas las páginas de filtro de informe según PivotField, el PivotField debe estar ubicado en PageFields. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | Mostrar todas las páginas de filtro de informe según el índice de posición en PageFields |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | Mostrar todas las páginas de filtro de informe según el nombre de PivotField, el PivotField debe estar ubicado en PageFields. |

### Ejemplos

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
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

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Cambiar los atributos de PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

// Agregar filtro dinámico
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

// Agregar condición de formato de pivote
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

//haz tu negocio

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Agregar filtro dinámico
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Agregar condición de formato de pivote
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Ver también

* espacio de nombres [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
