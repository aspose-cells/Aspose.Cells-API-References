---
title: "ExportObjectEvent.GetSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportObjectEvent‑metod. Hämtar objektet som ska exporteras"
type: docs
url: /sv/net/aspose.cells/exportobjectevent/getsource/
---
## ExportObjectEvent.GetSource method

Hämtar objektet som ska exporteras.

```csharp
public object GetSource()
```

### Returvärde

objektet som ska exporteras.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventMethodGetSourceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild för att demonstrera GetSource‑funktionaliteten
            int pictureIndex = worksheet.Pictures.Add(1, 1, "sample.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            try
            {
                // Skapa en anpassad export‑objekt‑lyssnare
                HtmlSaveOptions saveOptions = new HtmlSaveOptions
                {
                    ExportObjectListener = new CustomExportObjectListener()
                };

                // Spara arbetsboken för att utlösa ExportObjectEvent
                using (Stream stream = new FileStream("GetSourceDemo.html", FileMode.Create))
                {
                    workbook.Save(stream, saveOptions);
                }

                Console.WriteLine("GetSource method demonstrated successfully. Check the output HTML file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetSource: {ex.Message}");
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Demonstrera GetSource‑metoden
            object source = e.GetSource();

            if (source is Picture)
            {
                Console.WriteLine("GetSource returned a Picture object");
                return "custom-image-url.jpg";
            }

            return null;
        }
    }
}
```

### Se även

* class [ExportObjectEvent](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


