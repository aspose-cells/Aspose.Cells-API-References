---
title: "Worksheet.Workbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt das Arbeitsmappenobjekt zurück, das dieses Blatt enthält"
type: docs
url: /de/net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Ruft das Arbeitsmappen‑Objekt ab, das dieses Blatt enthält.

```csharp
public Workbook Workbook { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Quellarbeitsmappe und holen Sie ein Arbeitsblatt
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten zum Quellarbeitsblatt hinzu
            sourceSheet.Cells["A1"].PutValue("Sample Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            
            // Erstelle eine Ziel-Arbeitsmappe.
            Workbook destWorkbook = new Workbook();
            
            // Kopieren Sie das Design aus der Quellarbeitsmappe mithilfe der Worksheet.Workbook-Eigenschaft
            destWorkbook.CopyTheme(sourceSheet.Workbook);
            
            // Greifen Sie auf das Zielarbeitsblatt zu und kopieren Sie Daten
            Worksheet destSheet = destWorkbook.Worksheets[0];
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
            
            // Kopieren Sie Daten mit Formatierung
            destRange.Copy(sourceRange);
            
            // Speichere das Zielarbeitsbuch
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


