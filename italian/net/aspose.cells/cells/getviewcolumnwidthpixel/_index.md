---
title: "Cells.GetViewColumnWidthPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottieni la larghezza in diversi tipi di visualizzazione"
type: docs
url: /it/net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

Restituisce la larghezza in diversi tipi di visualizzazione.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | L'indice della colonna. |

### Valore di ritorno

la larghezza della colonna in unità di pixel

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il tipo di visualizzazione su PageLayoutView
            worksheet.ViewType = ViewType.PageLayoutView;
            
            // Imposta la larghezza della colonna in caratteri (verrà convertita in pixel)
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Ottieni la larghezza della colonna in pixel
            int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
            
            // Restituisci il risultato
            Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
            
            // Salva la cartella di lavoro
            workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


