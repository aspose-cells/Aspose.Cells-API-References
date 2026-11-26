---
title: "TextBoxOptions.TopMarginPt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "TextBoxOptions property. Получает и задает верхний отступ в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

Получает и задает верхний отступ в единицах точек.

```csharp
public double TopMarginPt { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить текстовое поле на лист
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Установите верхний отступ в точках
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // Сохраните книгу
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


