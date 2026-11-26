---
title: "TextBoxOptions.RightMarginPt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "TextBoxOptions property. Получает и задает правый отступ в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/rightmarginpt/
---
## TextBoxOptions.RightMarginPt property

Получает и задает правый отступ в единицах точек.

```csharp
public double RightMarginPt { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            int textBoxIndex = worksheet.TextBoxes.Add(1, 1, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "Sample Text";

            // Установите правый отступ в точках
            textBox.TextBoxOptions.RightMarginPt = 0.2d;

            // Сохраните книгу
            workbook.Save("TextBoxRightMarginDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


