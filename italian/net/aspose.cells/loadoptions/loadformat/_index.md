---
title: "LoadOptions.LoadFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene il formato di caricamento"
type: docs
url: /it/net/aspose.cells/loadoptions/loadformat/
---
## LoadOptions.LoadFormat property

Ottiene il formato di caricamento.

```csharp
public LoadFormat LoadFormat { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Crea file CSV di esempio
            File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");

            // Crea LoadOptions per il formato CSV e visualizza la proprietà
            LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
            Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

            // Carica CSV con le opzioni corrette
            Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
            Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);

            // Crea LoadOptions per il formato XLSX e visualizza la proprietà
            LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
            Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);

            // Crea/salva un file XLSX di esempio
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
            newWorkbook.Save("sample.xlsx");

            // Carica XLSX con le opzioni corrette
            Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
            Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);

            // Pulisci i file temporanei
            File.Delete("sample.csv");
            File.Delete("sample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


