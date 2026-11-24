---
title: "CopyOptions.CopyOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CopyOptions‑Konstruktor. CopyOptions‑Konstruktor"
type: docs
url: /de/net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

CopyOptions-Konstruktor.

```csharp
public CopyOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge ein Arbeitsblatt hinzu und erhalte das erste Arbeitsblatt
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            
            // Füge Beispieldaten zum Quellblatt hinzu
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            sourceSheet.Cells["A4"].PutValue(300);
            
            // Erstelle CopyOptions mit dem Konstruktor
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;
            
            // Kopiere Zeilen mit den Optionen
            destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
            
            // Speichere die Arbeitsmappe
            workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


