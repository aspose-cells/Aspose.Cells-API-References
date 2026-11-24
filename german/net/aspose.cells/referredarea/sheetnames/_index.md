---
title: "ReferredArea.SheetNames"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReferredArea-Eigenschaft. Namen aller Arbeitsblätter, auf die diese Instanz verweist"
type: docs
url: /de/net/aspose.cells/referredarea/sheetnames/
---
## ReferredArea.SheetNames property

Namen aller Arbeitsblätter, auf die diese Instanz verweist.

```csharp
public string[] SheetNames { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertySheetNamesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Daten hinzu, um eine Formelbezug zu erstellen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Formeln berechnen, um Referenzen zu erhalten
            workbook.CalculateFormula();

            // Den referenzierten Bereich aus der Formel in A3 abrufen
            ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];

            // Die SheetNames-Eigenschaft anzeigen
            Console.WriteLine("SheetNames referenced by the formula:");
            if (referredArea.SheetNames != null)
            {
                foreach (string sheetName in referredArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Ein weiteres Arbeitsblatt hinzufügen und einen bereichsübergreifenden Bezug erstellen
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=Sheet1!A3");

            // Formeln erneut berechnen
            workbook.CalculateFormula();

            // Den referenzierten Bereich aus der bereichsübergreifenden Formel abrufen
            ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];

            // SheetNames für bereichsübergreifenden Bezug anzeigen
            Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
            if (crossSheetArea.SheetNames != null)
            {
                foreach (string sheetName in crossSheetArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


