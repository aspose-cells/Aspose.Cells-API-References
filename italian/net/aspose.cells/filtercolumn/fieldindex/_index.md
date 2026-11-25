---
title: "FilterColumn.FieldIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Ottiene e imposta lo spostamento della colonna nell'intervallo"
type: docs
url: /it/net/aspose.cells/filtercolumn/fieldindex/
---
## FilterColumn.FieldIndex property

Ottiene e imposta lo spostamento della colonna nell'intervallo.

```csharp
public int FieldIndex { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Employees");
            worksheet.Cells["A2"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["A3"].PutValue("Marketing");
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["A4"].PutValue("IT");
            worksheet.Cells["B4"].PutValue(12);

            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:B4";
            
            // Aggiungi filtro alla prima colonna (Dipartimento)
            worksheet.AutoFilter.AddFilter(0, "Sales");

            // Ottieni la colonna del filtro
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            
            // Dimostra la proprietà FieldIndex
            Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
            
            // Aggiorna e salva
            worksheet.AutoFilter.Refresh();
            workbook.Save("FilterColumnFieldIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


