---
title: "Classe IconFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.IconFilter classe. Rappresenta il filtro icona"
type: docs
url: /it/net/aspose.cells/iconfilter/
---
## IconFilter class

Rappresenta il filtro icona.

```csharp
public class IconFilter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | Ottiene e imposta l'indice basato su zero di un'icona in un set di icone. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Ottiene e imposta quale set di icone è usato per questo criterio di filtro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Popola dati di esempio
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // Crea filtro automatico
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // Ottieni il filtro icona
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // Imposta le proprietà del filtro icona
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // Salva la cartella di lavoro
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon filter applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with IconFilter: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


