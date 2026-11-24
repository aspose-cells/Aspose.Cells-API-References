---
title: "PageSetup.PrintTitleColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Spalten an, die die Zellen enthalten, die auf der linken Seite jeder Seite wiederholt werden"
type: docs
url: /de/net/aspose.cells/pagesetup/printtitlecolumns/
---
## PageSetup.PrintTitleColumns property

Stellt die Spalten dar, die die Zellen enthalten, die auf der linken Seite jeder Seite wiederholt werden.

```csharp
public string PrintTitleColumns { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleColumnsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greife auf die Seiteneinrichtung zu
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Setze die Drucktitelspalten, damit Spalte A auf jeder gedruckten Seite wiederholt wird
            pageSetup.PrintTitleColumns = "$A:$A";
            
            // Füge einige Daten zu Spalte A hinzu, um die Wirkung zu demonstrieren
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PrintTitleColumnsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


