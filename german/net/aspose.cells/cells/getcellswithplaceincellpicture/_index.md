---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt alle Zellen zurück, die ein eingebettetes Bild enthalten."
type: docs
url: /de/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

Ermittelt alle Zellen, die ein eingebettetes Bild enthalten.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### Rückgabewert

Enumerator, um alle Cell-Objekte zu durchlaufen, die ein eingebettetes Bild enthalten.

### Hinweise

Wenn in diesem Arbeitsblatt kein Bild mit der Einstellung "Place in Cell" vorhanden ist, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Füge ein Bild zum Arbeitsblatt hinzu (dies wird von GetCellsWithPlaceInCellPicture nicht gezählt).
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // Füge ein eingebettetes Bild zu Zelle B3 hinzu (dies wird gezählt).
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // Entferne das schwebende Bild
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // Zellen mit eingebetteten Bildern abrufen
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // Speichern und neu laden, um die Persistenz zu überprüfen
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // Nach dem Neuladen überprüfen
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


