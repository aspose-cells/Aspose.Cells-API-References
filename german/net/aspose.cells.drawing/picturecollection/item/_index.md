---
title: "PictureCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PictureCollection property. Gibt das Picture-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Gibt das [`Picture`](../../picture/) Element am angegebenen Index zurück.

```csharp
public Picture this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bildersammlung abrufen
            PictureCollection pictures = worksheet.Pictures;
            
            // Füge ein Bild hinzu (ersetze "image.png" durch den tatsächlichen Bildpfad)
            int index = pictures.Add(1, 1, "image.png");
            
            // Greife auf das Bild über die Item-Eigenschaft zu
            Picture pic = pictures[index];
            
            // Demonstriere die Verwendung der Item-Eigenschaft
            Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
            
            // Bildeigenschaften ändern
            pic.Height = 200;
            pic.Width = 300;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PictureCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


