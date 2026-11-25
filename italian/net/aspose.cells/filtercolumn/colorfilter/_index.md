---
title: "FilterColumn.ColorFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Ottiene ColorFilter per filtrare i dati per colore"
type: docs
url: /it/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

Ottiene [`ColorFilter`](../../colorfilter/) per filtrare i dati per colore.

```csharp
public ColorFilter ColorFilter { get; }
```

### Osservazioni

Imposta [`FilterType`](../filtertype/) come ColorFilter per primo, altrimenti verrà restituito Null.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio con colori
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // Applica filtro automatico
                worksheet.AutoFilter.Range = "A1:A4";

                // Ottieni la colonna del filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Accedi alla proprietà ColorFilter (sola lettura)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // Visualizza le proprietà di ColorFilter
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // Salva la cartella di lavoro
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
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

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


