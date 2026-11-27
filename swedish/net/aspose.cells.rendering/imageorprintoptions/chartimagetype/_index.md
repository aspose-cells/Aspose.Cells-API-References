---
title: "ImageOrPrintOptions.ChartImageType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Egenskapen ImageOrPrintOptions. Ange diagrammets bildtyp vid konvertering. standardvärde PNG."
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/chartimagetype/
---
## ImageOrPrintOptions.ChartImageType property

Ange diagrammets bildtyp vid konvertering. standardvärde: PNG.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ChartImageType { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Istället renderas Chart och Shape alltid som vektorelement (t.ex. point, line) för renderingskvalitet. Denna egenskap kommer att tas bort 12 månader senare sedan juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyChartImageTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett kalkylblad med ett diagram.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:A4", true);

            try
            {
                // Skapa en ImageOrPrintOptions-instans
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visa det aktuella värdet för ChartImageType.
                Console.WriteLine("Current ChartImageType: " + options.ImageType);

                // Ange en annan bildtyp för diagramrendering.
                options.ImageType = ImageType.Png;
                Console.WriteLine("ChartImageType set to: " + options.ImageType);

                // Skapa en SheetRender för att demonstrera egenskapens effekt.
                SheetRender renderer = new SheetRender(worksheet, options);

                // Rendera diagrammet till en minnesström.
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Chart rendered successfully with ChartImageType: " + options.ImageType);
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Spara arbetsboken
                workbook.Save("ChartImageTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


