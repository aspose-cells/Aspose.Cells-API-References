---
title: "PictureCollection.Camera"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PictureCollection-Methode. Erstellt ein Foto des Bereichs"
type: docs
url: /de/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

Erstellt ein Foto des Bereichs.

```csharp
public int Camera(int row, int column, string range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex dieses Bildes. |
| column | Int32 | Der Spaltenindex dieses Bildes. |
| Bereich | String | Der Bereich, der fotografiert werden muss |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu, um einen Bereich zu erstellen
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // Rufen Sie die Pictures‑Sammlung aus dem Arbeitsblatt ab
                PictureCollection pictures = worksheet.Pictures;

                // Rufen Sie die Camera‑Methode auf, um ein Kamerabild zu erstellen
                // Parameter: row (obere linke Zeile), column (obere linke Spalte), range (Quellbereich)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


