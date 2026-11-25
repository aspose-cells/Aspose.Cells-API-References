---
title: "FilterColumn.IconFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Ottiene IconFilter per filtrare i dati per icona"
type: docs
url: /it/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

Ottiene `IconFilter` per filtrare i dati per icona.

```csharp
public IconFilter IconFilter { get; }
```

### Osservazioni

Prima di utilizzare questa proprietà, assicurati che [`FilterType`](../filtertype/) sia IconFilter, altrimenti verrà restituito null.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio con formattazione condizionale che utilizza icone
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // Applica il filtro automatico all'intervallo
                worksheet.AutoFilter.Range = "A1:A5";

                // Ottieni la colonna del filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Accedi alla proprietà IconFilter (sola lettura)
                IconFilter iconFilter = filterColumn.IconFilter;

                // Visualizza le proprietà di IconFilter se esiste
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // Salva la cartella di lavoro
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
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

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


