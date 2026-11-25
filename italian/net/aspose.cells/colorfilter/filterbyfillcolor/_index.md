---
title: "ColorFilter.FilterByFillColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ColorFilter. Indica se filtrare per il colore di riempimento delle celle"
type: docs
url: /it/net/aspose.cells/colorfilter/filterbyfillcolor/
---
## ColorFilter.FilterByFillColor property

Se filtrare per il colore di riempimento della cella.

```csharp
public bool FilterByFillColor { get; set; }
```

### Osservazioni

True: colore di riempimento della cella; False: colore del carattere della cella.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterPropertyFilterByFillColorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio con diversi colori di riempimento
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");

            // Imposta i colori di riempimento
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

            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;

            // Crea un filtro colore per il colore di riempimento
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, null);
            filter.Refresh();

            // Verifica le impostazioni del filtro
            FilterColumn filterColumn = filter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            // Dimostra la proprietà FilterByFillColor
            Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor); // Should be True
            Console.WriteLine("Filtered rows:");
            for (int row = 1; row <= 3; row++)
            {
                Console.WriteLine($"Row {row} hidden: {cells.IsRowHidden(row)}");
            }
        }
    }
}
```

### Vedi anche

* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


