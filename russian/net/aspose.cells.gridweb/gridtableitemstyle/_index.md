---
title: "Класс GridTableItemStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.GridTableItemStyle. Наследуется от System.Web.UI.WebControls.TableItemStyle. Инкапсулирует стили WebCell."
type: docs
url: /ru/net/aspose.cells.gridweb/gridtableitemstyle/
---
## GridTableItemStyle class

Наследуется от System.Web.UI.WebControls.TableItemStyle. Инкапсулирует стили WebCell.

```csharp
public class GridTableItemStyle : TableItemStyle, ISerializable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes/) { get; set; } | Атрибуты фонового изображения. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl/) { get; set; } | URL фонового изображения. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle/) { get; set; } | Указывает стиль нижней границы ячейки. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom/) { get; set; } | Получает или задаёт пользовательский формат, null или пустая строка означают отсутствие пользовательского формата. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel/) { get; set; } | Получает или задаёт уровень отступа. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked/) { get; set; } | Получает или задаёт значение, указывающее, может ли ячейка быть изменена, когда лист защищён. Когда лист защищён и IsLocked равно true, ячейка не может быть отредактирована. Когда лист защищён и IsLocked равно false, ячейка может быть отредактирована. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle/) { get; set; } | Указывает стиль левой границы ячейки. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype/) { get; set; } | Получает или задает формат отображения чисел и дат. Шаблоны форматирования различаются для разных регионов. |
| [QuotePrefix](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) { get; set; } | Указывает, начинается ли значение ячейки с одинарной кавычки. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle/) { get; set; } | Указывает стиль правой границы ячейки. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle/) { get; set; } | Получает или задаёт атрибут Rotation. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle/) { get; set; } | Указывает стиль верхней границы ячейки. |

## Методы

| Имя | Описание |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender/#addattributestorender_1)(HtmlTextWriter, WebControl) | Только для внутреннего использования. Метод реализации. Не вызывайте этот метод напрямую. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom/)(Style) | Копирует из другого объекта стиля. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode/)() | Служит хеш-функцией для конкретного типа, подходящей для использования в алгоритмах хеширования и структурах данных, таких как хеш-таблица. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith/)(Style) | Объединяет с другим объектом стиля. |

### Примеры

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

### См. также

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


