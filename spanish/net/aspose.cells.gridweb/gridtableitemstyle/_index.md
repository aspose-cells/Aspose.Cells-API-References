---
title: GridTableItemStyle
second_title: Referencia de API de Aspose.Cells para .NET
description: Heredado de System.Web.UI.WebControls.TableItemStyle. Encapsula los estilos de una WebCell.
type: docs
weight: 780
url: /es/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Heredado de System.Web.UI.WebControls.TableItemStyle. Encapsula los estilos de una WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle)() | Constructor por defecto. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes) { get; set; } | Atributos de imagen de fondo. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl) { get; set; } | URL de la imagen de fondo. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle) { get; set; } | Especifica el estilo del borde inferior de la celda. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom) { get; set; } | Obtiene o establece el formato personalizado, cadena nula o vacía significa que no hay formato personalizado. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel) { get; set; } | Obtiene o establece el nivel de sangría. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked) { get; set; } | Obtiene o establece un valor que indica si una celda se puede modificar o no cuando su hoja de trabajo está protegida. Cuando su hoja de trabajo está protegida y IsLocked es verdadero, la celda no se puede editar. Cuando su hoja de trabajo está protegida y IsLocked es falso, la celda se puede editar. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle) { get; set; } | Especifica el estilo del borde izquierdo de la celda. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype) { get; set; } | Obtiene o establece el formato de visualización de números y fechas. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle) { get; set; } | Especifica el estilo del borde derecho de la celda. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle) { get; set; } | Obtiene o establece el atributo Rotación. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle) { get; set; } | Especifica el estilo del borde superior de la celda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender#addattributestorender_1)(HtmlTextWriter, WebControl) | Solo para uso interno. Método de implementación No llamar directamente a este método. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom)(Style) | Copias de otro objeto de estilo. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode)() | Sirve como una función hash para un tipo particular, adecuado para usar en algoritmos hash y estructuras de datos como una tabla hash. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith)(Style) | Se fusiona con otro objeto de estilo. |

### Ejemplos

```csharp
[C#]
...
using System.Web.UI.WebControls;
...
...
WebWorksheets sheets = GridWeb1.WebWorksheets;
sheets.Clear();
WebWorksheet sheet = sheets[sheets.Add("demo1")];

WebCell cell = sheet.Cells[0,0];
cell.StringValue = "Demo Text";

Aspose.Cells.GridWeb.TableItemStyle style = cell.GetStyle();
style.Font.Size = new FontUnit("72pt");
style.Wrap = false;

style.BackColor = Color.Gray;
style.BorderStyle = BorderStyle.Solid;
style.BorderWidth = new Unit(1, UnitType.Pixel);
style.BorderColor = Color.Silver;

style.RightBorderStyle.BorderColor = Color.Black;
style.RightBorderStyle.BorderStyle = BorderStyle.Solid;
style.RightBorderStyle.BorderWidth = new Unit(1, UnitType.Pixel);
style.BottomBorderStyle.BorderColor = Color.Black;
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid;
style.BottomBorderStyle.BorderWidth = new Unit(1, UnitType.Pixel);
cell.SetStyle(style);

[Visual Basic]
...
Imports System.Web.UI.WebControls
...
...
Dim sheets As WebWorksheets =  GridWeb1.WebWorksheets
sheets.Clear()
Dim sheet As WebWorksheet =  sheets(sheets.Add(__0__))

Dim cell As WebCell =  sheet.Cells(0,0)
cell.StringValue = "Demo Text"

Dim style As Aspose.Cells.GridWeb.TableItemStyle = cell.GetStyle()
style.Font.Size = New FontUnit("72pt")
style.Wrap = False

style.BackColor = Color.Gray
style.BorderStyle = BorderStyle.Solid
style.BorderWidth = New Unit(1, UnitType.Pixel)
style.BorderColor = Color.Silver

style.RightBorderStyle.BorderColor = Color.Black
style.RightBorderStyle.BorderStyle = BorderStyle.Solid
style.RightBorderStyle.BorderWidth = New Unit(1, UnitType.Pixel)
style.BottomBorderStyle.BorderColor = Color.Black
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid
style.BottomBorderStyle.BorderWidth = New Unit(1, UnitType.Pixel)
cell.SetStyle(style)
```

### Ver también

* espacio de nombres [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* asamblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
