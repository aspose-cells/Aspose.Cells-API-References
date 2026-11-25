---
title: "Cells.GetRowHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'altezza delle righe"
type: docs
url: /it/net/aspose.cells/cells/getrowheight/
---
## GetRowHeight(int, bool, CellsUnitType) {#getrowheight_1}

Restituisce l'altezza della riga.

```csharp
public double GetRowHeight(int row, bool isOriginal, CellsUnitType unitType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| isOriginal | Booleano | Indica se restituisce l'altezza originale della riga o 0 per una riga nascosta. |
| unitType | CellsUnitType | Tipo di unità del valore di altezza restituito |

### Valore di ritorno

Altezza della riga

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'altezza della riga per la riga 3 (20 pixel)
            worksheet.Cells.SetRowHeightPixel(3, 20);
            
            // Ottieni l'altezza della riga in unità diverse
            double heightInPixels = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Pixel);
            double heightInPoints = worksheet.Cells.GetRowHeight(3, true, CellsUnitType.Point);
            
            // Restituisci i risultati
            Console.WriteLine("Row height in pixels: " + heightInPixels);
            Console.WriteLine("Row height in points: " + heightInPoints);
        }
    }
}
```

### Vedi anche

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRowHeight(int) {#getrowheight}

Restituisce l'altezza di una riga specificata, in unità di punti.

```csharp
public double GetRowHeight(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga |

### Valore di ritorno

Altezza della riga

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets["Sheet1"];
            Cells cells = ws.Cells;
            
            string strText = "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.";
            cells[0, 0].PutValue(strText);
            
            Style style = cells[0, 0].GetStyle();
            style.IsTextWrapped = true;
            cells[0, 0].SetStyle(style);
            
            ws.Cells.SetColumnWidth(0, 50);
            ws.AutoFitRows();
            
            double rowHeight = cells.GetRowHeight(0);
            Console.WriteLine("Row height: " + rowHeight);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


