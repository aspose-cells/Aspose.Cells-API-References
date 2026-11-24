---
title: "Workbook.CountOfStylesInPool"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt die Anzahl der Stile im Stilpool zurück"
type: docs
url: /de/net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Liest die Anzahl der Stile im Stil-Pool.

```csharp
public int CountOfStylesInPool { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCountOfStylesInPoolDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Anfängliche Anzahl der Stile im Pool ermitteln
            int initialStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Initial styles in pool: {initialStyleCount}");

            // Einige Stile hinzufügen, indem Zellen geändert werden
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Stil 1
            Style style1 = wb.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            cells["A1"].SetStyle(style1);
            
            // Stil 2
            Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            style2.Pattern = BackgroundType.Solid;
            cells["B1"].SetStyle(style2);

            // Aktualisierte Anzahl der Stile ermitteln
            int updatedStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Styles after modifications: {updatedStyleCount}");

            // Speichern, um die Stilpersistenz zu demonstrieren
            wb.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


