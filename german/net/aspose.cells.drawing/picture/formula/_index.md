---
title: "Picture.Formula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Picture-Eigenschaft. Liest und setzt die Daten der Formel"
type: docs
url: /de/net/aspose.cells.drawing/picture/formula/
---
## Picture.Formula property

Ruft die Daten der Formel ab und legt sie fest.

```csharp
public string Formula { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Formel für das Bild festlegen
            picture.Formula = "A1:A3";
            Console.WriteLine("Picture Formula: " + picture.Formula);

            // Formel ändern
            picture.Formula = "B1:B3";
            Console.WriteLine("Updated Picture Formula: " + picture.Formula);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


