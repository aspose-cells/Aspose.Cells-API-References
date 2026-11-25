---
title: "ImportTableOptions.CheckMergedCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Indica se controllare le celle unite"
type: docs
url: /it/net/aspose.cells/importtableoptions/checkmergedcells/
---
## ImportTableOptions.CheckMergedCells property

Indica se controllare le celle unite.

```csharp
public bool CheckMergedCells { get; set; }
```

### Esempi

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Customer1
    {
        public int CustomerId { get; set; }
        public string Name { get; set; }
    }

    public class ImportTableOptionsPropertyCheckMergedCellsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea celle unite per dimostrazione
            worksheet.Cells.Merge(3, 3, 2, 1); // Merge D4:D5
            worksheet.Cells[3, 3].PutValue("MergedValue");

            // Crea dati di esempio
            List<Customer1> customers = new List<Customer1>
            {
                new Customer1 { CustomerId = 1, Name = "Customer1" },
                new Customer1 { CustomerId = 2, Name = "Customer2" },
                new Customer1 { CustomerId = 3, Name = "Customer3" }
            };

            // Imposta le opzioni di importazione con CheckMergedCells abilitato
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = false,
                InsertRows = true,
                CheckMergedCells = true
            };

            // Importa dati
            worksheet.Cells.ImportCustomObjects(customers, 0, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Verifica che le celle unite siano state preservate
            Cell mergedCell = worksheet.Cells["D4"];
            Console.WriteLine($"Merged cell value: {mergedCell.StringValue}");
            Console.WriteLine($"Is cell merged: {mergedCell.IsMerged}");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


