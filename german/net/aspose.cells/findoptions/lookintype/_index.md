---
title: "FindOptions.LookInType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions-Eigenschaft. Typ, in dem gesucht wird"
type: docs
url: /de/net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

Im Typ nachsehen.

```csharp
public LookInType LookInType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookInTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Werte und Formeln in Zellen festlegen
            worksheet.Cells["A1"].PutValue("SearchValue");
            worksheet.Cells["A2"].Formula = "=A1";
            worksheet.Cells["B1"].PutValue("OtherValue");

            // Find-Optionen erstellen, um nur in Formeln zu suchen
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            // Nach dem Wert in Formeln suchen
            Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);

            // Gib das Ergebnis aus
            if (foundCell != null)
            {
                Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
            }
            else
            {
                Console.WriteLine("Value not found in formulas");
            }
        }
    }
}
```

### Siehe auch

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


