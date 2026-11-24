---
title: "ReferredArea.IsEntireRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReferredArea-Eigenschaft. Gibt an, ob dieser Bereich die gesamte Zeile (alle Spalten) enthält"
type: docs
url: /de/net/aspose.cells/referredarea/isentirerow/
---
## ReferredArea.IsEntireRow property

Gibt an, ob dieser Bereich alle Spalten (gesamte Zeile) enthält.

```csharp
public bool IsEntireRow { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Erstelle einen benannten Bereich, der sich auf die gesamte Zeile 2 bezieht
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$2:$2";

            // Hole den referenzierten Bereich des benannten Bereichs
            ReferredArea referredArea = workbook.Worksheets.Names["NamedRange1"].GetReferredAreas(false)[0];

            // Zeige den aktuellen Wert von IsEntireRow an
            Console.WriteLine("IsEntireRow value for NamedRange1: " + referredArea.IsEntireRow);

            // Erstelle einen weiteren benannten Bereich, der sich auf einen bestimmten Bereich bezieht (nicht die gesamte Zeile)
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // Den referenzierten Bereich des zweiten benannten Bereichs abrufen
            ReferredArea referredArea2 = workbook.Worksheets.Names["NamedRange2"].GetReferredAreas(false)[0];

            // Den aktuellen Wert von IsEntireRow für den zweiten Bereich anzeigen
            Console.WriteLine("IsEntireRow value for NamedRange2: " + referredArea2.IsEntireRow);

            // Demonstrieren Sie die Wirkung von IsEntireRow, indem Sie die Bereichsdimensionen prüfen
            Console.WriteLine("NamedRange1 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("NamedRange2 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // Speichere die Arbeitsmappe
            workbook.Save("ReferredAreaPropertyIsEntireRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


