---
title: "ReferredArea.SheetNames"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReferredArea. Nomi di tutti i fogli di lavoro a cui questa istanza fa riferimento"
type: docs
url: /it/net/aspose.cells/referredarea/sheetnames/
---
## ReferredArea.SheetNames property

Nomi di tutti i fogli di lavoro a cui fa riferimento questa istanza.

```csharp
public string[] SheetNames { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertySheetNamesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per creare un riferimento di formula
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Calcola le formule per ottenere i riferimenti
            workbook.CalculateFormula();

            // Ottieni l'area di riferimento dalla formula in A3
            ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];

            // Visualizza la proprietà SheetNames
            Console.WriteLine("SheetNames referenced by the formula:");
            if (referredArea.SheetNames != null)
            {
                foreach (string sheetName in referredArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Aggiungi un altro foglio di lavoro e crea un riferimento incrociato tra fogli
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=Sheet1!A3");

            // Calcola nuovamente le formule
            workbook.CalculateFormula();

            // Ottieni l'area di riferimento dalla formula tra fogli
            ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];

            // Visualizza i nomi dei fogli per il riferimento tra fogli
            Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
            if (crossSheetArea.SheetNames != null)
            {
                foreach (string sheetName in crossSheetArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


