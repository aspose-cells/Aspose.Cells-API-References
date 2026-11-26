---
title: "Класс TextBoxOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Texts.TextBoxOptions. Представляет текстовые параметры формы"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

Представляет параметры текста фигуры

```csharp
public class TextBoxOptions
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Разрешено ли переполнение текста за пределы формы. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Возвращает нижний отступ в единицах Points |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Получает и задает левый отступ в единицах точек. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Указывает, следует ли изменять размер формы, чтобы вместить текст |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Получает и задает правый отступ в единицах точек. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Получает или задает направление отображения текста внутри заданного текстового блока. Соответствует "Форматировать форму - Параметры текста - Текстовое поле - Направление текста" в Excel |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | Это соответствует "Format Shape - Text Options - Text Box - Vertical Alignment" в Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Получает и задает верхний отступ в единицах точек. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Указывает перенос текста внутри формы. False - перенос текста не будет происходить. True - перенос текста будет происходить. |

### Примеры

```csharp

[C#]
//Создание объекта Workbook
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//выполняйте свою работу

//Сохраните файл Excel.
workbook.Save("exmaple.xlsx");
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


