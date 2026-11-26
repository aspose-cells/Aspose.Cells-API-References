---
title: "Worksheet.TextBoxes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Возвращает коллекцию TextBox"
type: docs
url: /ru/net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

Возвращает коллекцию [`TextBox`](../../../aspose.cells.drawing/textbox/) коллекцию.

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTextBoxesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Добавить текстовое поле на лист
            int tID = ws.TextBoxes.Add(1, 1, 500, 1000);
            Aspose.Cells.Drawing.TextBox textBox = ws.TextBoxes[tID];

            // Установить текст и отформатировать его части
            textBox.Text = "Red text 1. Plain text 1. Red text 2. Plain text 2.";
            textBox.Characters(0, 10).Font.Color = Color.Red;
            textBox.Characters(26, 10).Font.Color = Color.DarkRed;

            // Сохраните книгу
            wb.Save("TextBoxExample.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


