---
title: "ImageOrPrintOptions.WarningCallback"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger varnings-callback"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/warningcallback/
---
## ImageOrPrintOptions.WarningCallback property

Hämtar eller anger varningsåteranrop.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till innehåll som kommer att generera en varning under rendering
            worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
            Style style = workbook.CreateStyle();
            style.Font.Name = "NonExistentFont";
            worksheet.Cells["A1"].SetStyle(style);

            // Skapa en ImageOrPrintOptions-instans
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Visa initialt WarningCallback-värde
            Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);

            // Skapa och tilldela anpassad varnings-callback
            var warningCallback = new RenderingWarningCallback();
            options.WarningCallback = warningCallback;

            // Skapa SheetRender för att demonstrera callback under rendering
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_image.png");

            // Kontrollera om varningar fångades
            Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
        }
    }

    // Anpassad callback-implementation för att hantera renderingsvarningar
    public class RenderingWarningCallback : IWarningCallback
    {
        public int WarningCount { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            // Hantera varningar för teckensnittssubstitution
            if (warningInfo.WarningType == WarningType.FontSubstitution)
            {
                Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
                WarningCount++;
            }
        }
    }
}
```

### Se även

* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


