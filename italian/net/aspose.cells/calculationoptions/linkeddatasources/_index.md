---
title: "CalculationOptions.LinkedDataSources"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. Specifica le origini dati per i collegamenti esterni utilizzati nelle formule"
type: docs
url: /it/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Specifica le origini dati per i collegamenti esterni utilizzati nelle formule.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Osservazioni

Come [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), qui è possibile specificare le origini dati per i collegamenti esterni utilizzati nelle formule da calcolare, in particolare quelli usati nella funzione INDIRECT. Per quei collegamenti esterni utilizzati nella funzione INDIRECT, non vengono considerati parte dei collegamenti esterni della cartella di lavoro e non possono essere aggiornati da [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). L'abbinamento di quelle cartelle di lavoro con i collegamenti esterni è determinato da [`FileName`](../../workbook/filename/) e [`DataSource`](../../externallink/datasource/). Pertanto, assicurati che [`FileName`](../../workbook/filename/) sia stato specificato con il valore corretto (in genere dovrebbe coincidere con il relativo [`DataSource`](../../externallink/datasource/)) per ogni cartella di lavoro affinché possano essere collegati come previsto.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro esterna con dati
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // Aggiungi intervalli denominati nella cartella di lavoro esterna
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // Crea la cartella di lavoro principale
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Imposta le formule che fanno riferimento alla cartella di lavoro esterna
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // Calcola le formule utilizzando LinkedDataSources
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

### Vedi anche

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


