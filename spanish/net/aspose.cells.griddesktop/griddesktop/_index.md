---
title: GridDesktop
second_title: Referencia de API de Aspose.Cells para .NET
description: Aspose GridDesktop class Representa un objeto raíz para crear un control GridDesktop. Para usar este control simplemente arrástrelo desde su caja de herramientas a un formulario o control de usuario.
type: docs
weight: 840
url: /es/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Aspose GridDesktop class Representa un objeto raíz para crear un control GridDesktop. Para usar este control, simplemente arrástrelo desde su caja de herramientas a un formulario o control de usuario.

```csharp
public class GridDesktop : UserControl
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridDesktop](griddesktop)() | Aspose GridDesktop class |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex) { get; set; } | Obtiene o establece el índice de la hoja seleccionada. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont) { get; set; } | Obtiene o establece la hoja activa que muestra la fuente de la barra de hojas. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas) { get; set; } | Obtiene o establece un valor que indica si necesitamos ejecutar todas las fórmulas, como cuando ejecutamos todas las fórmulas, cuando actualizamos el valor de una celda, y afecta a otros, y otros afectan a otros, cada vez más, porque todas las celdas necesitan volver a calcularse ,al igual que el efecto mariposa, necesita mucha operación de pila, obtendrá un rendimiento muy bajo, como en CELLSNET-41921, este problema contiene el mismo archivo que puede mostrar este escenario será mejor que ejecutemos todas las fórmulas, ,ya que cuando ejecutamos todas las fórmulas podemos tener alguna optimización. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle) { get; set; } | Indica el estilo del borde del control. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible) { get; set; } | Obtiene o establece un valor que indica si el encabezado de la columna está visible. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont) { get; set; } | Obtiene o establece la fuente de visualización predeterminada del texto del comentario. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager) { get; } | Obtiene la instancia de ContextMenuManager. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont) { get; set; } | Obtiene o establece la fuente por defecto de la celda |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor) { get; set; } | Obtiene o establece el color de fuente predeterminado de la celda. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste) { get; set; } | Indica si copiar/pegar según el portapapeles, para que pueda copiar/pegar con MS-EXCEL. Solo copia/pega el valor de la celda, no copia ninguna otra configuración de la celda como formato, estilo de borde, etc. El valor predeterminado es falso. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension) { get; set; } | Obtiene o establece un valor que indica si la operación de copia ampliará el número de filas o columnas. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption) { get; set; } | Obtiene o establece un valor que indica si la operación de copia copiará el valor del atributo CellLocked del estilo de una celda. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo) { get; set; } | Obtiene o establece un valor que indica si la función Deshacer está habilitada. El valor predeterminado es falso. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting) { get; set; } | Obtiene o establece la opción de memoria. |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible) { get; set; } | Establece la estatua visible para la barra de desplazamiento horizontal. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible) { get; set; } | Establece la estatua visible para Vertical ScrollBar. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names) { get; } | Obtiene la colección de todos los objetos Name en la hoja de cálculo. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows) { get; set; } | Establece u obtiene el tamaño de fila para Paginación. El máximo de PageRows admitido es 100000, el máximo de número de página admitido es 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype) { get; set; } | Indica qué tipo de pegado cuando se realiza la acción de pegar, solo disponible cuando EnableClipboardCopyPaste es falso . |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1) { get; set; } | Obtiene o establece un valor que indica si el control usa el estilo de referencia R1C1. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas) { get; set; } | Obtiene o establece un valor que indica si se debe volver a calcular la fórmula de todas las celdas cuando cambia el valor de una celda. El valor predeterminado es verdadero. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible) { get; set; } | Obtiene o establece un valor que indica si el encabezado de la fila está visible. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont) { get; set; } | Obtiene o establece la fuente de visualización predeterminada de la barra lateral. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible) { get; set; } | Obtiene o establece un valor que indica si la barra lateral está visible. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth) { get; set; } | Establece/Obtiene el ancho de la Hoja Tab. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu) { get; set; } | Obtiene o establece un valor que indica si el control puede mostrar el menú contextual. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus) { get; set; } | Obtiene o establece un valor que indica si mostrar el estado de cálculo El valor predeterminado es verdadero. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager) { get; } | Obtiene la instancia de UndoManager. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets) { get; } | Obtiene las hojas de trabajo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear)() | Borra el control de GridDesktop. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy)() | Copia el contenido de la celda enfocada al portapapeles. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut)() | Corta el contenido de la celda enfocada al portapapeles. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit)() | Establece vista dividida. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter)() | Notifica a GridDesktop que finalice FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile)(Stream) | Exporta a un flujo de archivo de Excel, incluido el flujo de E/S de disco o el flujo de memoria. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_2)(string) | Exporta a un archivo de Excel. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_1)(Stream, FileFormatType) | Exporta a un flujo de archivo de Excel, incluido el flujo de E/S de disco o el flujo de memoria. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_3)(string, FileFormatType) | Exporta a un archivo de Excel. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet)() | Obtiene la hoja de trabajo activa actual. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar)() | regresar barra de desplazamiento horizontal |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar)() | regresar barra de desplazamiento vertical |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile)(Stream) | Importaciones desde una secuencia de archivos de Excel, incluida la secuencia de archivos de disco o la secuencia de memoria. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_3)(string) | Importaciones desde un archivo de Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_1)(Stream, bool) | Importaciones desde una secuencia de archivos de Excel, incluida la secuencia de archivos de disco o la secuencia de memoria. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_4)(string, bool) | Importaciones desde un archivo de Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_5)(string, int) | Importa una hoja de cálculo desde un archivo de Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_2)(Stream, string, string, bool, bool) | Importaciones desde un archivo de Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_6)(string, string, string, bool, bool) | Importaciones desde un archivo de Excel. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog)(bool) | Abre el cuadro de diálogo FindReplace para buscar o reemplazar celdas. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste)() | Pega el contenido del portapapeles en la celda enfocada. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol)() | Actualizar el control GridDesktop. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas)() | Ejecuta la fórmula de todas las celdas. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible)() | Hace visibles todas las barras de desplazamiento. |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog)() | Abre un cuadro de diálogo de estilo, para establecer el estilo de las celdas, la fuente, los colores, etc. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter)(bool) | Notifica a GridDesktop para iniciar FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit)() | Desactivar vista dividida. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion)() | Obtener la versión de lanzamiento. |

## Campos

| Nombre | Descripción |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter) | las opciones para filtrar datos al cargar el libro de trabajo desde la plantilla. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage) | ya sea para mostrar el cuadro de mensaje cuando no se puede importar el archivo, el valor predeterminado es true |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns) | Ocurre después de eliminar la columna. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows) | Ocurre después de eliminar la fila. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns) | Ocurre después de insertar una nueva columna. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows) | Ocurre después de insertar una nueva fila. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate) | Ocurre antes de calcular la fórmula en el libro de trabajo. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile) | Ocurre antes de que el libro de trabajo se cargue desde el archivo. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick) | Ocurre cuando se hace clic en el botón de la celda. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged) | Ocurre cuando se cambia la propiedad Checkbox de la celda. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick) | Ocurre cuando se hace clic en la cuadrícula. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy) | Ocurre cuando se copia un ComboBox de celda de cuadrícula. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged) | Ocurre cuando se cambia la propiedad de datos de la celda de cuadrícula. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick) | Ocurre cuando se hace doble clic en la cuadrícula. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged) | Ocurre cuando el formato de celda se cambia a través del cuadro de diálogo Formato de celdas. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed) | Ocurre cuando se presiona una tecla mientras una celda tiene el foco. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged) | Ocurre cuando la propiedad del cuadro combinado de celdas SelectedIndex ha cambiado. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging) | Ocurre al escribir caracteres en una celda de cuadrícula. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed) | Ocurre cuando falla la validación de una celda de cuadrícula. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick) | Ocurre cuando se hace clic en el encabezado de la columna. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick) | Ocurre cuando se hace doble clic en el encabezado de la columna. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged) | Ocurre cuando los datos del comentario han cambiado. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate) | Ocurre después de calcular la fórmula en el libro de trabajo. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile) | Ocurre cuando se carga el libro. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged) | Ocurre cuando se cambia la celda enfocada. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged) | Ocurre cuando cambia el estado de ocultación de fila/columna. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent) | Ocurre después de seleccionar el elemento de filtro de fila. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick) | Ocurre cuando se hace clic en el encabezado de la fila. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick) | Ocurre cuando se hace doble clic en el encabezado de la fila. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged) | Ocurre cuando se cambia el rango de celdas seleccionado. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged) | Ocurre cuando se cambia la propiedad SelectedSheetIndex. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick) | Ocurre cuando se hace clic en la forma. |

### Observaciones

Consulte el documento .NET SDK para obtener más información sobre System.Windows.Forms.UserControl.

### Ejemplos

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### Ver también

* espacio de nombres [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
