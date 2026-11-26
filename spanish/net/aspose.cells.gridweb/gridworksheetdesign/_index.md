---
title: "Clase GridWorksheetDesign"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.GridWorksheetDesign clase. Heredada de GridWorksheet. Utilizada solo en tiempo de diseño."
type: docs
url: /es/net/aspose.cells.gridweb/gridworksheetdesign/
---
## GridWorksheetDesign class

Hereda de GridWorksheet. Solo se usa en tiempo de diseño.

```csharp
public class GridWorksheetDesign : GridWorksheet
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridWorksheetDesign](gridworksheetdesign/#constructor)() | Constructor predeterminado. |
| [GridWorksheetDesign](gridworksheetdesign/#constructor_1)(GridWorkbook) |  |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | Obtiene o establece la celda activa en la hoja de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | Obtiene y establece la imagen de fondo de la hoja de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | Vincula la colección de columnas.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | El objeto de origen de datos realmente enlazado en tiempo de ejecución. Es un objeto DataView cuando la propiedad DataSource es un objeto DataSet, DataTable o DataView.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar al origen de datos.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar al origen de datos.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | Obtiene la colección [`GridCell`](../../aspose.cells.gridweb.data/gridcell/).(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | Representa el nombre de código de la hoja de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | Obtiene la colección [`GridComment`](../../aspose.cells.gridweb.data/gridcomment/).(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | Obtiene el número de filas vinculadas en modo de enlace de datos.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | Obtiene o establece el DataMember del DataSource multi‑miembro. Generalmente representa un objeto DataTable de un DataSet.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | Obtiene o establece el DataSource. Generalmente es un objeto DataSet.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | Indica si la hoja de cálculo especificada se muestra de derecha a izquierda en lugar de izquierda a derecha. El valor predeterminado es false.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | True si se muestran valores cero.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | En modo de enlace de datos, indica si se deben crear los encabezados de columna vinculados en la hoja.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | Representa el índice de la primera columna visible.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | Representa el índice de la primera fila visible.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | Obtiene o establece la celda activa en la hoja de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | Obtiene la colección [`GridHyperlinkCollection`](../../aspose.cells.gridweb.data/gridhyperlinkcollection/).(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | Obtiene el índice de la hoja en la colección de hojas de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | Obtiene o establece un valor que indica si las líneas de la cuadrícula son visibles. El valor predeterminado es true.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | Obtiene o establece el nombre de la hoja de cálculo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | Indica si se muestra el esquema.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | Obtiene una colección de [`Pictures`](../../aspose.cells.gridweb.data/gridworksheet/pictures/).(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | Obtiene las pivotTables en la hoja de cálculo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | Indica si esta hoja de cálculo está seleccionada cuando se abre el libro de trabajo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | Obtiene una colección de [`Pictures`](../../aspose.cells.gridweb.data/gridworksheet/pictures/).(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de píxeles.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | Representa el color de la pestaña de la hoja de cálculo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | Obtiene el objeto [`GridWorkbook`](../../aspose.cells.gridweb.data/gridworkbook/) de la colección de hojas de cálculo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | Representa el factor de escala en porcentaje. Debe estar entre 10 y 400.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | Establece el rango al que se aplica el AutoFilter especificado.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | Agrega un filtro personalizado para la fila especificada.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/)(int) | Ajusta automáticamente el ancho de la columna.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/)(int, int, int) | Ajusta automáticamente el ancho de la columna.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() | (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/)(int) | Ajusta automáticamente la altura de la fila.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/)(int, int, int) | Ajusta automáticamente la altura de la fila.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/)(int, int, int, int) | Ajusta automáticamente la altura de la fila en un rango rectangular.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/)() | Ajusta automáticamente todas las filas en esta hoja de cálculo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/)(bool) | Ajusta automáticamente todas las filas en esta hoja de cálculo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/)(int, int) | Ajusta automáticamente la altura de la fila en un rango.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | Calcula una fórmula.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | Cancela y elimina la fila vinculada recién añadida.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | Borra todos los comentarios en la hoja de cálculo del diseñador.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | Confirma la fila vinculada recién añadida y la agrega a la fuente de datos.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | Copia el contenido y los formatos de otra hoja de cálculo.(Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | Después de establecer una fuente de datos para la hoja de cálculo, llame a este método para generar las columnas vinculadas automáticamente.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | Crea una nueva fila vinculada y la vincula a la fuente de datos.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[]) | Crea un subtotal en la hoja.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crea un subtotal en la hoja.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | Vincula la hoja a la DataSource.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | Vincula la hoja a la DataSource.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | Elimina una fila vinculada.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | Establece el filtro para la columna. Nota: debemos llamar a AddAutoFilter antes de llamar a filterString. La cadena de criterios del filtro. Nota: usamos la coma-&gt;"," como carácter separador, por lo que el valor de celda que desea filtrar no debe contener comas. filterString(10,\"123,456\") significa que la columna 10 debe contener 123 o 456, filterString(10,\"123\") significa que la columna 10 debe contener 123. El índice de columna se separa con comas, p. ej. 123,456,789 o abc(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/)(string, int, int) | Congela paneles en la celda especificada de la hoja de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/)(int, int, int, int) | Congela paneles en la celda especificada de la hoja de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | Obtiene el título de la columna. Si el título no está establecido, devuelve una cadena vacía.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | Obtiene el texto de información sobre herramientas del encabezado de columna.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | Obtiene si una columna es de solo lectura. este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | Obtiene los paneles congelados.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | Obtiene si la celda es de solo lectura. este es un atributo extendido de GridWeb, no se conservará en el archivo Excel real(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | Obtiene el título de la fila. Si el título no está establecido, devuelve una cadena vacía.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | Obtiene el texto de información sobre herramientas del encabezado de fila.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | Obtiene si una fila es de solo lectura. este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | Agrupa filas.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | Indica si la hoja de cálculo está protegida.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | Mueve la hoja a otra ubicación en la hoja de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | Actualiza los filtros automáticos para ocultar o mostrar las filas.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | Elimina el filtro automático de la hoja de cálculo.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | Elimina el subtotal creado por el método CreateSubtotal en la hoja.(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | El desplazamiento entero del campo al que desea aplicar, basado en la primera columna de filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0).(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | Hace que todas las celdas sean editables. este es un atributo extendido(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | Hace que todas las celdas sean de solo lectura. este es un atributo extendido, tenga en cuenta que este atributo no se conserva en la celda real; si desea mantener la protección, use setProtect(Heredado de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/).) |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | Establece el título de la columna. Tenga en cuenta que este es un atributo de extensión y no se puede conservar en el archivo de Excel (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | Establece el texto de información sobre herramientas del encabezado de columna (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | Establece una columna como solo lectura para que el usuario no pueda eliminarla del lado del cliente. Este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | Hace que un rango de celdas sea editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Haz que todas las celdas sean de solo lectura llamando al método SetAllCellsReadonly. Luego llama a este método para especificar el rango de celdas que deben ser editables (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | Establece si la celda es de solo lectura. Este es un atributo extendido de GridWeb, no se conservará en el archivo Excel real (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | Protege la hoja de cálculo (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | Hace que un rango de celdas sea de solo lectura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Primero haz que todas las celdas sean editables llamando al método SetAllCellsEditable. Luego llama a este método para especificar el rango de celdas que debe ser de solo lectura (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | Establece el título de la fila (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | Establece el texto de información sobre herramientas del encabezado de fila (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | Establece una fila como solo lectura para que el usuario no pueda eliminarla del lado del cliente. Este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | Descongela los paneles en la hoja de cálculo (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | Desagrupa filas (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | Desprotege la hoja de cálculo (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |

## Eventos

| Nombre | Descripción |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | Ocurre cuando la hoja de cálculo ha creado una nueva fila vinculada y necesita inicializarla (Hereda de [`GridWorksheet`](../../aspose.cells.gridweb.data/gridworksheet/)). |

### Ver también

* class [GridWorksheet](../../aspose.cells.gridweb.data/gridworksheet/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


