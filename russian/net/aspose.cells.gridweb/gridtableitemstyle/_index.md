---
title: GridTableItemStyle
second_title: Справочник по Aspose.Cells для .NET API
description: Унаследовано от System.Web.UI.WebControls.TableItemStyle. Инкапсулирует стили WebCell.
type: docs
weight: 780
url: /ru/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Унаследовано от System.Web.UI.WebControls.TableItemStyle. Инкапсулирует стили WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes) { get; set; } | Атрибуты фонового изображения. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl) { get; set; } | URL фонового изображения. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle) { get; set; } | Задает стиль нижней границы ячейки. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom) { get; set; } | Получает или задает пользовательский формат, нулевая или пустая строка означает отсутствие пользовательского формата. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel) { get; set; } | Получает или устанавливает уровень отступа. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked) { get; set; } | Получает или задает значение, указывающее, можно ли изменять ячейку, когда ее рабочий лист защищен. Когда рабочий лист защищен и IsLocked имеет значение true, ячейку нельзя редактировать. Когда его рабочий лист защищен, а IsLocked имеет значение false, ячейку можно редактировать. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle) { get; set; } | Задает стиль левой границы ячейки. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype) { get; set; } | Получает или задает формат отображения чисел и дат. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle) { get; set; } | Задает стиль правой границы ячейки. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle) { get; set; } | Получает или устанавливает атрибут вращения. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle) { get; set; } | Задает стиль верхней границы ячейки. |

## Методы

| Имя | Описание |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender#addattributestorender_1)(HtmlTextWriter, WebControl) | Только для внутреннего использования. Метод реализации Не вызывайте этот метод напрямую. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom)(Style) | Копирует из другого объекта стиля. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode)() | Служит хеш-функцией для определенного типа, подходящей для использования в алгоритмах хеширования и структурах данных, таких как хеш-таблица. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith)(Style) | Сливается с другим объектом стиля. |

### Примеры

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

### Смотрите также

* пространство имен [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* сборка [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
