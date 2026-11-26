---
title: "Clase GridWorksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.Data.GridWorksheet class. Encapsula el objeto que representa una sola hoja de cálculo"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

Encapsula el objeto que representa una sola hoja de cálculo.

```csharp
public class GridWorksheet : Control, ISerializable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | Obtiene o establece la celda activa en la hoja de cálculo. |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | Obtiene y establece la imagen de fondo de la hoja de cálculo. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | Vincule la colección de columnas. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | El objeto de origen de datos realmente enlazado en tiempo de ejecución. Es un objeto DataView cuando la propiedad DataSource es un objeto DataSet, DataTable o DataView. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar al origen de datos. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar al origen de datos. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | Obtiene la colección de [`GridCell`](../gridcell/). |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | Representa el nombre de código de la hoja de cálculo. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | Obtiene la colección [`GridComment`](../gridcomment/). |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | Obtiene el número de filas vinculadas en modo de enlace de datos. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | Obtiene o establece el DataMember del DataSource de múltiples miembros. Generalmente representa un objeto DataTable de un DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | Obtiene o establece el DataSource. Generalmente es un objeto DataSet. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. El valor predeterminado es false. |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | True si se muestran valores cero. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | En modo de enlace de datos, indica si se deben crear los encabezados de columna vinculados en la hoja. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | Representa el índice de la primera columna visible. |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | Representa el índice de la primera fila visible. |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | Obtiene o establece la celda activa en la hoja de cálculo. |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | Obtiene la colección [`GridHyperlinkCollection`](../gridhyperlinkcollection/). |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | Obtiene el índice de la hoja en la colección de hojas de cálculo. |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | Obtiene o establece un valor que indica si las líneas de la cuadrícula son visibles. El valor predeterminado es true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | Obtiene o establece el nombre de la hoja de cálculo. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | Indica si se muestra el contorno. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | Obtiene una colección [`Pictures`](./pictures/). |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | Obtiene las pivotTables en la hoja de cálculo. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | Indica si esta hoja de cálculo está seleccionada cuando se abre el libro de trabajo. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | Obtiene una colección [`Pictures`](./pictures/). |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de píxeles. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | Representa el color de la pestaña de la hoja. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | Obtiene el objeto [`GridWorkbook`](../gridworkbook/) de la colección de hojas de cálculo. |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | Representa el factor de escala en porcentaje. Debe estar entre 10 y 400. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | Establece el rango al que se aplica el AutoFilter especificado. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | Agregar filtro personalizado para la fila especificada. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn)(int) | Ajusta automáticamente el ancho de la columna. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Ajusta automáticamente el ancho de la columna. |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() |  |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow)(int) | Ajusta automáticamente la altura de la fila. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_1)(int, int, int) | Ajusta automáticamente la altura de la fila. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_2)(int, int, int, int) | Ajusta automáticamente la altura de la fila en un rango rectangular. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows)() | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_1)(bool) | Ajusta automáticamente todas las filas en esta hoja de cálculo. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_2)(int, int) | Ajusta automáticamente la altura de la fila en un rango. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | Calcula una fórmula. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | Cancela y elimina la fila vinculada recién añadida. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | Elimina todos los comentarios en la hoja de cálculo del diseñador. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | Confirma la fila vinculada recién añadida y la agrega al datasource. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | Copia contenidos y formatos de otra hoja de cálculo. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | Después de establecer un datasource para la hoja de cálculo, llame a este método para generar automáticamente las columnas vinculadas. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | Crea una nueva fila vinculada y la enlaza al datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Crea un subtotal en la hoja. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crea un subtotal en la hoja. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | Vincula la hoja al DataSource. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | Vincula la hoja al DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | Elimina una fila vinculada. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | Establece el filtro para la columna. Observe que debemos llamar a AddAutoFilter antes de llamar a filterString. La cadena de criterios de filtro. Observe que usamos la coma-&gt;"," como carácter separador, por lo que el valor de celda que desea filtrar no debe contener comas. filterString(10,"123,456") significa que la columna 10 debe contener 123 o 456, filterString(10,"123") significa que la columna 10 debe contener 123. El índice de columna se separa con comas, p. ej. 123,456,789 o abc. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes_1)(string, int, int) | Congela paneles en la celda especificada de la hoja de cálculo. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes)(int, int, int, int) | Congela paneles en la celda especificada de la hoja de cálculo. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | Obtiene el título de la columna. Si el título no está establecido, devuelve una cadena vacía. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | Obtiene el texto de información sobre herramientas del encabezado de columna. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | Obtiene si una columna es de solo lectura. Este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real. |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | Obtiene los paneles congelados. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | Obtiene si la celda es de solo lectura. Este es un atributo extendido de GridWeb, no se conservará en el archivo Excel real. |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | Obtiene el título de la fila. Si el título no está establecido, devuelve una cadena vacía. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | Obtiene el texto de información sobre herramienta del encabezado de fila. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | Obtiene si una fila es de solo lectura. este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | Agrupa filas. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | Indica si la hoja de cálculo está protegida. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | Mueve la hoja a otra ubicación en la hoja de cálculo. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | Actualiza los autofiltros para ocultar o mostrar las filas. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | Elimina el filtro automático de la hoja de cálculo. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | Elimina el subtotal creado por el método CreateSubtotal en la hoja. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | El desplazamiento entero del campo al que desea aplicar, basado en la primera columna de filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | Hace que todas las celdas sean editables.este es un atributo extendido |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | Hace que todas las celdas sean de solo lectura.este es un atributo extendido, tenga en cuenta que este atributo no se conserva en la celda real, si desea mantener la protección, use setProtect |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | Establece el título para la columna.por favor, tenga en cuenta que este es un atributo de extensión y no se conserva en el archivo Excel |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | Establece el texto de información sobre herramienta del encabezado de columna. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | Establece una columna como de solo lectura para que el usuario no pueda eliminarla desde el lado del cliente. este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | Hace que un rango de celdas sea editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Haga que todas las celdas sean de solo lectura llamando al método SetAllCellsReadonly. luego llame a este método para especificar el rango de celdas que deben ser editables |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | Establece si la celda es de solo lectura.este es un atributo extendido de GridWeb, no se conservará en el archivo Excel real |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | Protege la hoja de cálculo. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | Hace que un rango de celdas sea de solo lectura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Primero haga que todas las celdas sean editables llamando al método SetAllCellsEditable. luego llame a este método para especificar el rango de celdas que deben ser de solo lectura |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | Establece el título para la fila. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | Establece el texto de información sobre herramienta del encabezado de fila. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | Establece una fila como de solo lectura para que el usuario no pueda eliminarla desde el lado del cliente. este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | Descongela los paneles en la hoja de cálculo. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | Desagrupa filas. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | Desprotege la hoja de cálculo. |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | Ocurre cuando la hoja de cálculo ha creado una nueva fila vinculada y necesita inicializarla. |

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


