---
title: "ColorFilter.GetColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ColorFilter. Ottiene il colore di questo filtro"
type: docs
url: /it/net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

Ottiene il colore di questo filtro.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fogli | WorksheetCollection |  |

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterMethodGetColorWithWorksheetCollectionDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");
            
            // Crea filtro automatico
            worksheet.AutoFilter.Range = "A1:A4";
            
            // Crea filtro colore
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            worksheet.AutoFilter.Refresh();
            
            // Ottieni il filtro colore e verifica il suo colore
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            if (colorFilter != null)
            {
                Color retrievedColor = colorFilter.GetColor(workbook.Worksheets);
                Console.WriteLine("Filter color: " + retrievedColor.ToString());
            }
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


