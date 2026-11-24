---
title: "WorksheetCollection.Dxfs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Gibt die Master-Differenzformatierungsdatensätze zurück"
type: docs
url: /de/net/aspose.cells/worksheetcollection/dxfs/
---
## WorksheetCollection.Dxfs property

Ruft die Master-Differenzformatierungsdatensätze ab.

```csharp
public DxfCollection Dxfs { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyDxfsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Bedingung und Stil festlegen
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            fcc[0].Style = style;
            
            // Demonstriere die Dxfs-Eigenschaft
            Console.WriteLine("Dxfs count before applying formatting: " + workbook.Worksheets.Dxfs.Count);
            
            // Formatierung anwenden, die zu Dxfs hinzugefügt wird
            worksheet.ConditionalFormattings[0][0].Priority = 1;
            
            Console.WriteLine("Dxfs count after applying formatting: " + workbook.Worksheets.Dxfs.Count);
        }
    }
}
```

### Siehe auch

* class [DxfCollection](../../dxfcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


