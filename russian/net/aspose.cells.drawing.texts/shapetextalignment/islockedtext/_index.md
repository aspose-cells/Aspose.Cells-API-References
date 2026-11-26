---
title: "ShapeTextAlignment.IsLockedText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeTextAlignment. Указывает, заблокирована ли форма, когда лист защищён"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/islockedtext/
---
## ShapeTextAlignment.IsLockedText property

Указывает, заблокирована ли фигура, когда лист защищён.

```csharp
public bool IsLockedText { get; set; }
```

### Примечания

Работает только когда лист защищён.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsLockedTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text";

            // Получить свойства выравнивания текста
            Aspose.Cells.Drawing.Texts.ShapeTextAlignment textAlignment = textBox.TextBody.TextAlignment;

            // Установить и продемонстрировать свойство IsLockedText
            textAlignment.IsLockedText = true;
            Console.WriteLine("Text locked status: " + textAlignment.IsLockedText);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


