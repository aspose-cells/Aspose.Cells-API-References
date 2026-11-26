---
title: "Перечисление MsoDrawingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.MsoDrawingType. Представляет тип объектов офисных рисунков"
type: docs
url: /ru/net/aspose.cells.drawing/msodrawingtype/
---
## MsoDrawingType enumeration

Представляет тип объектов офисного рисунка.

```csharp
public enum MsoDrawingType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Group | `0` | Группа |
| Line | `1` | Линия |
| Rectangle | `2` | Прямоугольник |
| Oval | `3` | Овал |
| Arc | `4` | Дуга |
| Chart | `5` | Диаграмма |
| TextBox | `6` | Текстовое поле |
| Button | `7` | Кнопка |
| Picture | `8` | Изображение |
| Polygon | `9` | Многоугольник |
| CheckBox | `11` | Флажок |
| RadioButton | `12` | Радиокнопка |
| Label | `14` | Метка |
| DialogBox | `15` | Диалоговое окно |
| Spinner | `16` | Спиннер |
| ScrollBar | `17` | Полоса прокрутки |
| ListBox | `18` | Список |
| GroupBox | `19` | Групповой элемент |
| ComboBox | `20` | Выпадающий список |
| Comment | `25` | Комментарий |
| OleObject | `24` | OleObject |
| CellsDrawing | `30` | Только для сохранения объекта рисунка в файле шаблона. |
| Unknown | `29` | Только для сохранения объекта рисунка в файле xlsx. |
| Slicer | `31` | Slicer |
| WebExtension | `32` | Веб-расширение |
| SmartArt | `33` | Smart Art |
| CustomXml | `34` | Пользовательская XML-форма, например Ink. |
| Timeline | `35` | Хронология |
| Model3D | `36` | 3D-модель |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoDrawingTypeDemo
    {
        public static void MsoDrawingTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру на лист
            Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
            rectangle.Name = "MyRectangle";
            rectangle.AlternativeText = "This is a rectangle shape";

            // Добавить овальную форму на лист
            Shape oval = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 5, 0, 5, 0, 100, 200);
            oval.Name = "MyOval";
            oval.AlternativeText = "This is an oval shape";

            // Добавить линейную форму на лист
            Shape line = worksheet.Shapes.AddShape(MsoDrawingType.Line, 8, 0, 8, 0, 100, 200);
            line.Name = "MyLine";
            line.AlternativeText = "This is a line shape";

            // Добавить форму текстового поля на лист
            Shape textBox = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 11, 0, 11, 0, 100, 200);
            textBox.Name = "MyTextBox";
            textBox.AlternativeText = "This is a textbox shape";
            textBox.Text = "Hello, Aspose.Cells!";

            // Вывести имена и типы форм
            foreach (Shape shape in worksheet.Shapes)
            {
                Console.WriteLine($"Shape Name: {shape.Name}, Shape Type: {shape.MsoDrawingType}");
            }

            // Сохраните книгу
            workbook.Save("MsoDrawingTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


