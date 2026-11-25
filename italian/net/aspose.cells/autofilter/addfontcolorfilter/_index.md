---
title: "AutoFilter.AddFontColorFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Aggiunge un filtro di colore del carattere"
type: docs
url: /it/net/aspose.cells/autofilter/addfontcolorfilter/
---
## AutoFilter.AddFontColorFilter method

Aggiunge un filtro di colore del carattere.

```csharp
public void AddFontColorFilter(int fieldIndex, CellsColor color)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| color | CellsColor | L'oggetto [`CellsColor`](../../cellscolor/). |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFontColorFilterWithInt32CellsColorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio con diversi colori del carattere
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Item 1");
            cells["A3"].PutValue("Item 2");
            cells["A4"].PutValue("Item 3");
            
            // Imposta i colori del carattere
            Style style = cells["A2"].GetStyle();
            style.Font.Color = Color.Red;
            cells["A2"].SetStyle(style);
            
            style = cells["A3"].GetStyle();
            style.Font.Color = Color.Blue;
            cells["A3"].SetStyle(style);
            
            style = cells["A4"].GetStyle();
            style.Font.Color = Color.Green;
            cells["A4"].SetStyle(style);

            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Crea un filtro di colore per carattere rosso
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            
            // Aggiungi filtro di colore del carattere
            filter.AddFontColorFilter(0, cr);
            filter.Refresh();
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFilterFontColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


