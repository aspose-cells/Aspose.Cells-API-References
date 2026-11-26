---
title: "Clase GridDesktop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridDesktop.GridDesktop. La clase Aspose GridDesktop representa un objeto raíz para crear un control GridDesktop. Para usar este control simplemente arrástralo desde tu caja de herramientas a un formulario o control de usuario"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

La clase Aspose GridDesktop representa un objeto raíz para crear un control GridDesktop. Para usar este control, simplemente arrástralo desde tu caja de herramientas a un formulario o control de usuario.

```csharp
public class GridDesktop : UserControl
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridDesktop](griddesktop/)() | Clase Aspose GridDesktop |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | Obtiene o establece el índice de la hoja seleccionada. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | Obtiene o establece la fuente mostrada en la barra de la hoja activa. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | Obtiene o establece un valor que indica si necesitamos ejecutar todas las fórmulas, ya que al ejecutar todas las fórmulas, al actualizar el valor de una celda, afecta a otras, y esas a otras, y así sucesivamente, lo que hace que todas las celdas necesiten recalcularse, como el efecto mariposa, requiere muchas operaciones de pila, lo que produce un rendimiento muy bajo, como en CELLSNET-41921; este problema contiene el archivo que muestra este escenario. Es mejor ejecutar todas las fórmulas, ya que al hacerlo podemos aplicar algunas optimizaciones. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | Indica el estilo del borde para el control. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | Obtiene o establece un valor que indica si el encabezado de columna es visible. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | Obtiene o establece la fuente predeterminada para mostrar el texto de los comentarios. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | Obtiene la instancia de ContextMenuManager. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | Obtiene o establece la fuente predeterminada de la celda |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | Obtiene o establece el color de fuente predeterminado de la celda. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | Indica si se debe copiar/pegar basándose en el portapapeles, de modo que pueda copiar/pegar con MS-EXCEL. Solo copia/pega el valor de la celda; no copia ninguna otra configuración de la celda como formato, estilo de borde, etc. El valor predeterminado es false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | Obtiene o establece un valor que indica si la operación de copia ampliará el número de filas o columnas. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | Obtiene o establece un valor que indica si la operación de copia copiará el valor del atributo CellLocked del estilo de una celda. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | Obtiene o establece un valor que indica si la función Deshacer está habilitada. El valor predeterminado es false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | Obtiene o establece la opción de memoria, el valor predeterminado es GridMemorySetting.Normal |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | Establece el estado visible para la barra de desplazamiento horizontal. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | Establece el estado visible para la barra de desplazamiento vertical. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | Obtiene la colección de todos los objetos Name en la hoja de cálculo. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | Establece u obtiene el tamaño de fila para la paginación. El máximo de PageRows admitido es 100000, el máximo de número de página admitido es 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | Indica qué tipo de pegado se usa al realizar la acción de pegar, solo disponible cuando EnableClipboardCopyPaste es false. El valor predeterminado es GridPasteType.Default; |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | Obtiene o establece un valor que indica si el control utiliza el estilo de referencia R1C1. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | Obtiene o establece un valor que indica si se deben recalcular todas las fórmulas de las celdas cuando el valor de una celda cambia. El valor predeterminado es true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | Obtiene o establece un valor que indica si el encabezado de fila es visible. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | Obtiene o establece la fuente predeterminada de visualización de la barra de hoja. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | Obtiene o establece un valor que indica si la barra de hoja es visible. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | Establece u obtiene el ancho de la pestaña de hoja. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | Obtiene o establece un valor que indica si el control puede mostrar el menú contextual. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | Establece u obtiene si se muestra el mensaje de error o advertencia al establecer el valor de la fórmula de la celda, el valor predeterminado es true. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | Establece u obtiene si se muestra el símbolo de triángulo para la celda que contiene una cadena numérica pero está almacenada en formato de texto. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | Obtiene o establece un valor que indica si se muestra el estado de cálculo. El valor predeterminado es true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | Obtiene la instancia de UndoManager. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | Obtiene las hojas de cálculo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | Limpia el control GridDesktop. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | Copia el contenido de la celda enfocada al portapapeles. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | Corta el contenido de la celda enfocada al portapapeles. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | Establece la vista dividida. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | Notifica a GridDesktop que finalice el FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | Exporta a un flujo de archivo Excel, incluyendo flujo de E/S de disco o flujo de memoria. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | Exporta a un archivo Excel. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | Exporta a un flujo de archivo Excel, incluyendo flujo de E/S de disco o flujo de memoria. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | Exporta a un archivo Excel. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | Exporta a un flujo de archivo PDF, incluyendo flujo de E/S de disco o flujo de memoria. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | Exporta a un flujo de archivo PDF, incluyendo flujo de E/S de disco o flujo de memoria. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | Obtiene la hoja de cálculo activa actual. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | devuelve la barra de desplazamiento horizontal |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | devuelve la barra de desplazamiento vertical |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | Importa desde un archivo Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | Importa desde un archivo Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | Importa una hoja de cálculo desde un archivo Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | Importa desde un archivo Excel. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | Importa desde un archivo Excel. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | Anular invalidación. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | Abre el cuadro de diálogo BuscarReemplazar para buscar o reemplazar celdas. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | Pega el contenido del portapapeles en la celda enfocada. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | Actualiza el control GridDesktop. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | Ejecuta todas las fórmulas de las celdas. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | Establece todas las barras de desplazamiento visibles. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | Establece un gestor de recursos personalizado para implementar la localización definida por el usuario |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | Abre un cuadro de diálogo de estilo, para establecer el estilo, la fuente, los colores, etc., de las celdas. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | Notifica a GridDesktop para iniciar el Pintor de Formato. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | Desactivar vista dividida. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | Obtiene la versión de lanzamiento. |

## Campos

| Nombre | Descripción |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | las opciones para filtrar datos al cargar el libro de trabajo desde una plantilla. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | si mostrar un cuadro de mensaje cuando falle la importación del archivo, el valor predeterminado es verdadero. |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | Ocurre después de que se elimina una columna. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | Ocurre después de que se elimina una fila. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | Ocurre después de que se inserta una nueva columna. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | Ocurre después de que se inserta una nueva fila. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | Ocurre antes de calcular la fórmula en el libro de trabajo. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | Ocurre antes de que el libro de trabajo se cargue desde un archivo. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | Ocurre cuando se hace clic en el botón de la celda. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | Ocurre cuando se cambia la propiedad Checked del checkbox de la celda. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | Ocurre cuando se hace clic en la celda de la cuadrícula. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | Ocurre cuando se está copiando un ComboBox de celda de cuadrícula. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | Ocurre cuando se cambia la propiedad de datos de la celda de la cuadrícula. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | Ocurre cuando se hace doble clic en la celda de la cuadrícula. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | Ocurre cuando se cambia el formato de la celda mediante el cuadro de diálogo Formatear celdas. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | Ocurre cuando se presiona una tecla mientras una celda tiene el foco. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | Ocurre cuando la propiedad SelectedIndex del combobox de la celda ha cambiado. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | Ocurre al escribir caracteres en una celda de la cuadrícula. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | Ocurre cuando la validación de una celda de la cuadrícula falla. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | Ocurre cuando se hace clic en el encabezado de columna. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | Ocurre cuando se hace doble clic en el encabezado de columna. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | Ocurre cuando los datos del comentario han cambiado. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | Ocurre después de calcular la fórmula en el libro de trabajo. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | Ocurre cuando se carga el libro de trabajo. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | Ocurre cuando se cambia la celda con foco. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | Ocurre cuando se hace clic en la forma. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | Ocurre cuando cambia el estado de ocultación de fila/columna. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | Ocurre después de seleccionar un elemento del filtro de fila. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | Ocurre cuando se hace clic en el encabezado de fila. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | Ocurre cuando se hace doble clic en el encabezado de fila. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | Ocurre cuando se cambia el rango de celdas seleccionado. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | Ocurre cuando se cambia la propiedad SelectedSheetIndex. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | Ocurre cuando se hace clic en la forma. |

### Observaciones

Consulte la documentación del SDK de .NET para obtener más información sobre System.Windows.Forms.UserControl.

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

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


