---
title: "PowerQueryFormulaItem.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaItem-Eigenschaft. Gibt den Namen des Elements zurück"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaitem/name/
---
## PowerQueryFormulaItem.Name property

Ermittelt den Namen des Elements.

```csharp
public string Name { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemPropertyNameDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für Power Query hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            
            // Speichern, um die Erstellung von Power Query auszulösen
            string sourcePath = "pq_source.xlsx";
            workbook.Save(sourcePath);
            
            // Erneut öffnen, um auf Power Query-Formeln zuzugreifen
            workbook = new Workbook(sourcePath);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            
            // Power Query-Formeln verarbeiten
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula formula in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine("Formula Name: " + formula.Name);
                
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                {
                    Console.WriteLine("  Item Name: " + item.Name);
                    
                    // Demonstrieren Sie die Verwendung der Name-Eigenschaft
                    if (item.Name == "Source")
                    {
                        Console.WriteLine("Original Value: " + item.Value);
                        item.Value = "ModifiedSource";
                        Console.WriteLine("Modified Value: " + item.Value);
                    }
                }
            }
            
            // Modifizierte Arbeitsmappe speichern
            workbook.Save("pq_modified.xlsx");
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


