---
title: "Picture.DisplayAsIcon"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Wahr, wenn das angegebene Objekt als Symbol angezeigt wird und das Bild nicht automatisch geändert wird"
type: docs
url: /de/net/aspose.cells.drawing/picture/displayasicon/
---
## Picture.DisplayAsIcon property

True, wenn das angegebene Objekt als Symbol angezeigt wird und das Bild nicht automatisch geändert wird.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Setze die DisplayAsIcon-Eigenschaft auf wahr
            picture.DisplayAsIcon = true;
            
            // Setze weitere Bild-Eigenschaften
            picture.Name = "IconDisplay";
            picture.Height = 100;
            picture.Width = 100;

            // Speichere die Arbeitsmappe
            workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon display picture.");
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


