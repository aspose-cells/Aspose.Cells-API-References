---
title: "AutoFilter.AddFillColorFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Aggiunge un filtro di colore di riempimento"
type: docs
url: /it/net/aspose.cells/autofilter/addfillcolorfilter/
---
## AutoFilter.AddFillColorFilter method

Aggiunge un filtro di colore di riempimento.

```csharp
public void AddFillColorFilter(int fieldIndex, BackgroundType pattern, CellsColor foregroundColor, 
    CellsColor backgroundColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| modello | BackgroundType | Il tipo di modello di sfondo. |
| foregroundColor | CellsColor | Il colore di primo piano. |
| backgroundColor | CellsColor | Il colore di sfondo. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFillColorFilterWithInt32BackgroundTypeCellsColorCDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio con diversi colori di riempimento
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");
            
            // Applica diversi colori di riempimento
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);
            
            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);
            
            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Crea filtro automatico
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Crea colore delle celle per il filtraggio
            CellsColor filterColor = workbook.CreateCellsColor();
            filterColor.Color = Color.Red;
            
            // Applica filtro di colore di riempimento
            filter.AddFillColorFilter(0, BackgroundType.Solid, filterColor, filterColor);
            filter.Refresh();
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFilterFillColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BackgroundType](../../backgroundtype/)
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


