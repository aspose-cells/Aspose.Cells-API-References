---
title: "PivotTable.DataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene e imposta la fonte dati della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/datasource/
---
## PivotTable.DataSource property

Ottiene e imposta l'origine dati della pivot table.

```csharp
public string[] DataSource { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataSourceDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Accedi e visualizza le informazioni della fonte dati
            string[] dataSource = pivotTable.DataSource;
            Console.WriteLine("Pivot Table Data Sources:");
            foreach (string source in dataSource)
            {
                Console.WriteLine(source);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableDataSourceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


