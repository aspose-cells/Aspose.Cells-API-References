---
title: "FontSettingCollection.TextAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSettingCollection. Представляет настройку выравнивания текста тела"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/textalignment/
---
## FontSettingCollection.TextAlignment property

Представляет настройку выравнивания тела текста.

```csharp
public ShapeTextAlignment TextAlignment { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            shape.Text = "Sample Text";

            // Получайте и изменяйте свойства TextAlignment
            var textAlignment = shape.TextBody.TextAlignment;
            
            Console.WriteLine("Default Margins (Points):");
            Console.WriteLine($"AutoMargin: {textAlignment.IsAutoMargin}");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");

            // Изменить поля
            textAlignment.TopMarginPt = 36;
            textAlignment.BottomMarginPt = 36;
            textAlignment.LeftMarginPt = 18;
            textAlignment.RightMarginPt = 18;

            // Сохраните книгу
            workbook.Save("TextAlignmentDemo.xlsx");

            Console.WriteLine("\nModified Margins (Points):");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");
        }
    }
}
```

### См. также

* class [ShapeTextAlignment](../../shapetextalignment/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


