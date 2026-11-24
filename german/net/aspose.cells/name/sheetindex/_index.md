---
title: "Name.SheetIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Eigenschaft. Gibt an, dass dieser Name zu einer Arbeitsmappe oder einem Arbeitsblatt gehört. 0 = globaler Name, sonst Index zum Blatt (einsbasiert)"
type: docs
url: /de/net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Gibt an, ob dieser Name zu einer Arbeitsmappe oder einem Arbeitsblatt gehört. 0 = Globaler Name, sonst Index zum Blatt (einsbasiert).

```csharp
public int SheetIndex { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertySheetIndexDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Einige Arbeitsblätter hinzufügen
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Erstellen Sie einen benannten Bereich in Sheet2
            Worksheet sheet2 = workbook.Worksheets["Sheet2"];
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet2!$A$1:$B$10";
            
            // Zeigen Sie den Blatt-Index des benannten Bereichs an
            Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
            
            // Speichere die Arbeitsmappe
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


