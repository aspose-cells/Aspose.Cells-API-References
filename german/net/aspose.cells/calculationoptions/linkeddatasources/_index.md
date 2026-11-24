---
title: "CalculationOptions.LinkedDataSources"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationOptions-Eigenschaft. Gibt die Datenquellen für externe Links an, die in Formeln verwendet werden"
type: docs
url: /de/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Gibt die Datenquellen für in Formeln verwendete externe Verknüpfungen an.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Hinweise

Wie bei [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/) können Sie hier Datenquellen für externe Links angeben, die in Formeln verwendet und berechnet werden sollen, insbesondere solche, die in der INDIRECT‑Funktion verwendet werden. Für externe Links, die in der INDIRECT‑Funktion verwendet werden, werden sie nicht als Teil der externen Links des Arbeitsbuchs betrachtet und können nicht durch [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/) aktualisiert werden. Die Zuordnung dieser Arbeitsbücher zu externen Links wird durch [`FileName`](../../workbook/filename/) und [`DataSource`](../../externallink/datasource/) bestimmt. Bitte stellen Sie daher sicher, dass [`FileName`](../../workbook/filename/) für jedes Arbeitsbuch mit dem richtigen Wert angegeben wurde (in der Regel sollte er mit dem entsprechenden [`DataSource`](../../externallink/datasource/) übereinstimmen), damit sie wie erwartet verknüpft werden können.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // Externes Arbeitsbuch mit Daten erstellen
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // Benannte Bereiche in externer Arbeitsmappe hinzufügen
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // Hauptarbeitsmappe erstellen
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Formeln festlegen, die auf externe Arbeitsmappe verweisen
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // Formeln mit LinkedDataSources berechnen
            CalculationOptions options = new CalculationOptions();
            options.LinkedDataSources = new Workbook[] { wbExt };
            
            Console.WriteLine("Before calculation:");
            PrintCellValues(sheet);

            wb.CalculateFormula(options);
            
            Console.WriteLine("\nAfter calculation:");
            PrintCellValues(sheet);
        }

        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


