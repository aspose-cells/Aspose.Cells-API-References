---
title: "CellRichValue.Image"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellRichValue-egenskap. Hämtar bilddata för cellen"
type: docs
url: /sv/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

Hämtar bilddata för cellen.

```csharp
public virtual byte[] Image { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class CellRichValuePropertyImageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i kalkylbladet
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Hämta cellens rikvärde som innehåller bilden
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // Åtkomst till rikvärdet
            CellRichValue richValue = cell.GetRichValue();

            // Visa bildegenskaper
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // Ställ in ny alt‑text för bilden
            richValue.AltText = "Sample product image";

            // Spara arbetsboken
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


