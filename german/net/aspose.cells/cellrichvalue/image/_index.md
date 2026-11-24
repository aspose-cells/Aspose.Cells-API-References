---
title: "CellRichValue.Image"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellRichValue-Eigenschaft. Ruft die Bilddaten der Zelle ab"
type: docs
url: /de/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

Liest die Bilddaten der Zelle.

```csharp
public virtual byte[] Image { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Den Rich-Wert der Zelle abrufen, der das Bild enthält
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // Auf den Rich-Wert zugreifen
            CellRichValue richValue = cell.GetRichValue();

            // Bildeigenschaften anzeigen
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // Neuen Alternativtext für das Bild festlegen
            richValue.AltText = "Sample product image";

            // Speichere die Arbeitsmappe
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


