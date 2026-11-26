---
title: "TextOptions.FarEastName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextOptions. Получает и задает имя FarEast"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

Получает и задает название FarEast.

```csharp
public string FarEastName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFarEastNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму и задайте шрифт FarEastName
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            shape.Text = "Sample Text";
            shape.TextOptions.FarEastName = "宋体";

            // Сохраните и перезагрузите для проверки
            string outputPath = "output_FarEastName.xlsx";
            workbook.Save(outputPath);

            // Перезагрузить для проверки
            Workbook verifyWorkbook = new Workbook(outputPath);
            Aspose.Cells.Drawing.Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("FarEastName: " + verifyShape.TextOptions.FarEastName);
        }
    }
}
```

### См. также

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


