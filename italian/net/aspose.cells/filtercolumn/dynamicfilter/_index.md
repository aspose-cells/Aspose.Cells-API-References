---
title: "FilterColumn.DynamicFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Ottiene DynamicFilter per filtrare con criteri dinamici"
type: docs
url: /it/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

Ottiene `DynamicFilter` per filtrare con criteri dinamici.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### Osservazioni

Prima di utilizzare questa proprietà, assicurati che [`FilterType`](../filtertype/) sia DynamicFilter, altrimenti verrà restituito null.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // Applica filtro automatico
                worksheet.AutoFilter.Range = "A1:A4";

                // Ottieni la colonna del filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Accedi alla proprietà DynamicFilter (sola lettura)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // Visualizza le proprietà DynamicFilter
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // Salva la cartella di lavoro
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


