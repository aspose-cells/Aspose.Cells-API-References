---
title: "Clase WorksheetDesign"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.WorksheetDesign clase. Heredada de WebWorksheet. Utilizada solo en tiempo de diseño."
type: docs
url: /es/net/aspose.cells.gridweb/worksheetdesign/
---
## WorksheetDesign class

Hereda de WebWorksheet. Solo se usa en tiempo de diseño.

```csharp
public class WorksheetDesign : WebWorksheet
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WorksheetDesign](worksheetdesign/#constructor)() | Constructor predeterminado. |
| [WorksheetDesign](worksheetdesign/#constructor_1)(MainWeb, GridWorksheet) | el constructor con MainWeb y GridWorksheet |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Colección de columnas de enlace.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | El objeto de origen de datos realmente enlazado en tiempo de ejecución. Es un objeto DataView cuando la propiedad DataSource es un objeto DataSet, DataTable o DataView.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar al origen de datos.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | En modo de enlace de datos, BindStartRow y BindStartColumn indican la posición de la cuadrícula para enlazar al origen de datos.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } | (Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Obtiene los [`WebCells`](../../aspose.cells.gridweb.data/webcells/).(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } | (Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Obtiene el número de filas enlazadas en modo de enlace de datos.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Obtiene o establece el DataMember del DataSource multi‑miembro. Generalmente representa un objeto DataTable de un DataSet.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Obtiene o establece el DataSource. Generalmente es un objeto DataSet.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | En modo de enlace de datos, indica si se deben crear los encabezados de columna enlazados en la hoja.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Obtiene la colección HyperlinkCollection.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Obtiene el índice de sí mismo dentro de las hojas de cálculo.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Obtiene o establece si la hoja de cálculo está protegida. Cuando una hoja está protegida, todas las celdas no pueden editarse excepto la celda cuya propiedad IsLocked es false.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Obtiene o establece el nombre de la hoja.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } | (Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Indica si el nombre de esta hoja se muestra en las pestañas de hoja del control.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int) | Ajusta automáticamente el ancho de la columna.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/)(int, int, int) | Ajusta automáticamente el ancho de la columna. Este método ajusta automáticamente una columna basándose en el contenido de un rango de celdas dentro de la columna desde startRow hasta endRow. AutoFitColumn es una función imprecisa.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Cancela y elimina la fila vinculada recién añadida.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Confirma la nueva fila vinculada añadida y la agrega a la fuente de datos.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Copia de otro objeto de hoja de cálculo.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | Después de establecer una fuente de datos para la hoja de cálculo, llame a este método para generar las columnas vinculadas automáticamente.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Crea una nueva fila vinculada y la enlaza a la fuente de datos.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Crea un subtotal en la hoja.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Vincula la hoja a la Fuente de Datos.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Elimina una fila vinculada.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Congela paneles en la celda especificada de la hoja de cálculo.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int) | Agrupa filas.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/)(int, int, bool) | Agrupa filas.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Hace que todas las celdas sean editables. este es un atributo extendido(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Hace que todas las celdas sean solo lectura. este es un atributo extendido, aviso: este atributo no se puede mantener en la celda real, si desea mantener la protección, por favor use setProtect(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Hace que un rango de celdas sea editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Haga que todas las celdas sean solo lectura llamando al método SetAllCellsReadonly. luego llame a este método para especificar el rango de celdas que deben ser editables(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Hace que un rango de celdas sea solo lectura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Primero haga que todas las celdas sean editables llamando al método SetAllCellsEditable. luego llame a este método para especificar el rango de celdas que deben ser solo lectura(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Descongela paneles en la hoja de cálculo.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Desagrupa filas.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Actualiza el valor de la propiedad del registro de la fuente de datos vinculada según el valor de la celda.(Hereda de [`WebWorksheet`](../../aspose.cells.gridweb.data/webworksheet/).) |

### Ver también

* class [WebWorksheet](../../aspose.cells.gridweb.data/webworksheet/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


