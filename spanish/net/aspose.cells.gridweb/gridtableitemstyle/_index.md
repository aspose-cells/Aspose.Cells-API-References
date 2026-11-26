---
title: "Clase GridTableItemStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.GridTableItemStyle. Heredada de System.Web.UI.WebControls.TableItemStyle. Encapsula los estilos de un WebCell."
type: docs
url: /es/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Hereda de System.Web.UI.WebControls.TableItemStyle. Encapsula los estilos de un WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle, ISerializable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle/)() | Constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes/) { get; set; } | Atributos de la imagen de fondo. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl/) { get; set; } | URL de la imagen de fondo. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle/) { get; set; } | Especifica el estilo del borde inferior de la celda. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom/) { get; set; } | Obtiene o establece el formato personalizado; null o cadena vacía significa que no hay formato personalizado. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel/) { get; set; } | Obtiene o establece el nivel de sangría. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked/) { get; set; } | Obtiene o establece un valor que indica si una celda puede modificarse o no cuando su hoja de cálculo está protegida. Cuando la hoja está protegida y IsLocked es verdadero, la celda no puede editarse. Cuando la hoja está protegida y IsLocked es falso, la celda puede editarse. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle/) { get; set; } | Especifica el estilo del borde izquierdo de la celda. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype/) { get; set; } | Obtiene o establece el formato de visualización de números y fechas. Los patrones de formato son diferentes según la región. |
| [QuotePrefix](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) { get; set; } | Indica si el valor de la celda comienza con una comilla simple. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle/) { get; set; } | Especifica el estilo del borde derecho de la celda. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle/) { get; set; } | Obtiene o establece el atributo Rotación. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle/) { get; set; } | Especifica el estilo del borde superior de la celda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender/#addattributestorender_1)(HtmlTextWriter, WebControl) | Solo para uso interno. Método de implementación. No llame a este método directamente. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom/)(Style) | Copia de otro objeto de estilo. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode/)() | Funciona como una función hash para un tipo particular, adecuada para su uso en algoritmos de hash y estructuras de datos como una tabla hash. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith/)(Style) | Fusiona con otro objeto de estilo. |

### Ejemplos

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheetCollection sheets = GridWeb1.WorkSheets;

GridWorksheet sheet = sheets.Add("demo1");

sheet.Cells[0,0].PutValue("Demo Text");
GridTableItemStyle style = sheet.Cells[0, 0].Style;

style.Font.Size = wui.WebControls.FontUnit.Point(72);
style.Wrap = false;

style.BackColor = Color.Gray;
style.BorderStyle = wui.WebControls.BorderStyle.Solid;
style.BorderWidth = wui.WebControls.Unit.Pixel(1);
style.BorderColor = Color.Silver;
style.RightBorderStyle.BorderColor = Color.Black;
style.RightBorderStyle.BorderStyle = wui.WebControls.BorderStyle.Solid;
style.RightBorderStyle.BorderWidth = wui.WebControls.Unit.Pixel(1);
style.BottomBorderStyle.BorderColor = Color.Black;
style.BottomBorderStyle.BorderStyle = wui.WebControls.BorderStyle.Solid;
style.BottomBorderStyle.BorderWidth = wui.WebControls.Unit.Pixel(1);
sheet.Cells[0, 0].Style=style;
[Visual Basic]
Dim sheets As GridWorksheetCollection =  GridWeb1.WorkSheets
Dim sheet As GridWorksheet =  sheets(sheets.Add(__0__))

Dim cell As GridCell =  sheet.Cells(0,0)
cell.StringValue = "Demo Text"

Dim style As GridTableItemStyle = cell.GetStyle()
style.Font.Size = FontUnit.Point(72)
style.Wrap = False

style.BackColor = Color.Gray
style.BorderStyle = BorderStyle.Solid
style.BorderWidth = Unit.Pixel(1)
style.BorderColor = Color.Silver

style.RightBorderStyle.BorderColor = Color.Black
style.RightBorderStyle.BorderStyle = BorderStyle.Solid
style.RightBorderStyle.BorderWidth = Unit.Pixel(1)
style.BottomBorderStyle.BorderColor = Color.Black
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid
style.BottomBorderStyle.BorderWidth = Unit.Pixel(1)
cell.SetStyle(style)
```

### Ver también

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


