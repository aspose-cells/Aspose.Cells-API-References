---
title: "PictureCollection.Camera"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PictureCollection-metoden. Tar ett foto av området"
type: docs
url: /sv/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

Tar ett foto av området.

```csharp
public int Camera(int row, int column, string range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet för den här bilden. |
| column | Int32 | Kolumnindexet för den här bilden. |
| område | String | Området som kräver fotografering |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata för att skapa ett område
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // Hämta Pictures-samlingen från kalkylbladet
                PictureCollection pictures = worksheet.Pictures;

                // Anropa Camera-metoden för att skapa en kamerabild
                // Parametrar: rad (övre vänstra raden), kolumn (övre vänstra kolumnen), område (källområde)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // Spara arbetsboken
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


