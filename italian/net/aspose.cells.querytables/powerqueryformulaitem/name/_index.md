---
title: "PowerQueryFormulaItem.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaItem. Ottiene il nome dell'elemento"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaitem/name/
---
## PowerQueryFormulaItem.Name property

Ottiene il nome dell'elemento.

```csharp
public string Name { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemPropertyNameDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati Power Query di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            
            // Salva per avviare la creazione di Power Query
            string sourcePath = "pq_source.xlsx";
            workbook.Save(sourcePath);
            
            // Riapri per accedere alle formule Power Query
            workbook = new Workbook(sourcePath);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            
            // Elabora le formule Power Query
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula formula in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine("Formula Name: " + formula.Name);
                
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                {
                    Console.WriteLine("  Item Name: " + item.Name);
                    
                    // Dimostra l'uso della proprietà Name
                    if (item.Name == "Source")
                    {
                        Console.WriteLine("Original Value: " + item.Value);
                        item.Value = "ModifiedSource";
                        Console.WriteLine("Modified Value: " + item.Value);
                    }
                }
            }
            
            // Salvare la cartella di lavoro modificata
            workbook.Save("pq_modified.xlsx");
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


