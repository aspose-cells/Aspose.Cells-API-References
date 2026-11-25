---
title: "DataSorter.AddColorKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DataSorter. Aggiunge una chiave di ordinamento per colore"
type: docs
url: /it/net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

Aggiunge una chiave di ordinamento per colore.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | Int32 | L'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...) |
| type | SortOnType | Il tipo di valore di colore ordinato. |
| ordine | SortOrder | L'ordine di ordinamento. |
| colore | Color | Il colore di ordinamento personalizzato. |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddColorKeyWithInt32SortOnTypeSortOrderColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con celle colorate
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(7);
            
            // Applica colori alle celle
            Style styleRed = workbook.CreateStyle();
            styleRed.ForegroundColor = Color.Red;
            styleRed.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(styleRed);
            
            Style styleBlue = workbook.CreateStyle();
            styleBlue.ForegroundColor = Color.Blue;
            styleBlue.Pattern = BackgroundType.Solid;
            worksheet.Cells["A3"].SetStyle(styleBlue);
            
            Style styleGreen = workbook.CreateStyle();
            styleGreen.ForegroundColor = Color.Green;
            styleGreen.Pattern = BackgroundType.Solid;
            worksheet.Cells["A4"].SetStyle(styleGreen);

            // Crea l'ordinatore dei dati e aggiungi la chiave di colore
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);

            // Ordina i dati
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A4"));

            // Genera i valori ordinati (per dimostrazione)
            Console.WriteLine("Sorted values:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].IntValue);
            }
        }
    }
}
```

### Vedi anche

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


