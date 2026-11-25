---
title: "Enum FilterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.FilterType enum. Il tipo di filtro"
type: docs
url: /it/net/aspose.cells/filtertype/
---
## FilterType enumeration

Il tipo di filtro.

```csharp
public enum FilterType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| ColorFilter | `0` | Filtra per colore di riempimento della cella. |
| CustomFilters | `1` | Tipo di filtro personalizzato. |
| DynamicFilter | `2` | Tipo di filtro dinamico. |
| MultipleFilters | `3` | Quando vengono scelti più valori da filtrare, o quando viene scelto un gruppo di valori di data da filtrare, questo elemento raggruppa tali criteri insieme. |
| IconFilter | `4` | Filtra per icona della formattazione condizionale. |
| Top10 | `5` | Filtro Top 10. |
| None | `6` | Nessun filtro. |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Color");
            worksheet.Cells["A2"].PutValue("Red");
            worksheet.Cells["A3"].PutValue("Green");
            worksheet.Cells["A4"].PutValue("Blue");
            
            // Crea filtro automatico
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Crea filtro colore
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            
            // Aggiungi filtro colore alla colonna
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Verifica il tipo di filtro
            FilterColumn filterColumn = filter.FilterColumns[0];
            Console.WriteLine("Filter Type: " + filterColumn.FilterType);
            
            // Verifica le proprietà del filtro colore
            if (filterColumn.FilterType == FilterType.ColorFilter)
            {
                ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
                Console.WriteLine("Filter by fill color: " + colorFilter.FilterByFillColor);
                Console.WriteLine("Filter color: " + colorFilter.GetColor(workbook.Worksheets));
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


