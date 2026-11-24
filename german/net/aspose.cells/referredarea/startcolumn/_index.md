---
title: "ReferredArea.StartColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReferredArea-Eigenschaft. Die Startspalte des Bereichs"
type: docs
url: /de/net/aspose.cells/referredarea/startcolumn/
---
## ReferredArea.StartColumn property

Die Startspalte des Bereichs.

```csharp
public int StartColumn { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["C1"].PutValue("Cherry");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);

            // Erstelle einen benannten Bereich, der sich auf B1:C2 bezieht
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!B1:C2";

            // Hole den referenzierten Bereich mit recalculate auf false gesetzt
            ReferredArea referredArea = name.GetReferredAreas(false)[0];

            // Demonstriere die StartColumn-Eigenschaft
            Console.WriteLine("Start Column: " + referredArea.StartColumn);
            Console.WriteLine("End Column: " + referredArea.EndColumn);

            // Gib Werte im referenzierten Bereich unter Verwendung von StartColumn aus
            Cells cells = worksheet.Cells;
            for (int row = referredArea.StartRow; row <= referredArea.EndRow; row++)
            {
                for (int col = referredArea.StartColumn; col <= referredArea.EndColumn; col++)
                {
                    Console.WriteLine(cells[row, col].Name + ": " + cells[row, col].Value);
                }
            }
        }
    }
}
```

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


