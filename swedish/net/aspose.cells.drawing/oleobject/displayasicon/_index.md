---
title: "OleObject.DisplayAsIcon"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject egenskap. Sant om det angivna objektet visas som en ikon och bilden inte kommer att ändras automatiskt"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

Sant om det angivna objektet visas som en ikon och bilden inte kommer att ändras automatiskt.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OLE-objekt (PDF) i kalkylbladet
            byte[] pdfData = File.ReadAllBytes("example.pdf");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
            
            // Hämta OLE-objektet
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.ProgID = "AcroExch.Document.DC";
            
            // Demonstrera DisplayAsIcon-egenskapen
            oleObject.DisplayAsIcon = true; // Show as icon
            // oleObject.DisplayAsIcon = false; // Visa innehåll om möjligt
            
            // Spara arbetsboken
            workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


