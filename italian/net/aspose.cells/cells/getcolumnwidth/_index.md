---
title: "Cells.GetColumnWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene la larghezza della colonna"
type: docs
url: /it/net/aspose.cells/cells/getcolumnwidth/
---
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}

Restituisce la larghezza della colonna.

```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | L'indice della colonna. |
| isOriginal | Booleano | Indica se si sta ottenendo la larghezza originale. |
| unitType | CellsUnitType |  |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la larghezza della colonna per la colonna 1 (indice base 0)
            cells.SetColumnWidth(0, 20);

            // Ottieni la larghezza della colonna in diverse unità e modalità
            double widthInPixels = cells.GetColumnWidth(0, true, CellsUnitType.Pixel);
            double widthInPoints = cells.GetColumnWidth(0, true, CellsUnitType.Point);
            double defaultWidth = cells.GetColumnWidth(0, false, CellsUnitType.Pixel);

            Console.WriteLine("Column width in pixels: " + widthInPixels);
            Console.WriteLine("Column width in points: " + widthInPoints);
            Console.WriteLine("Default column width: " + defaultWidth);
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

## GetColumnWidth(int) {#getcolumnwidth}

Restituisce la larghezza (in unità di caratteri) della colonna specificata nella visualizzazione normale

```csharp
public double GetColumnWidth(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna |

### Valore di ritorno

Larghezza della colonna. Per i fogli di calcolo, la larghezza della colonna è misurata come il numero di caratteri della larghezza massima delle cifre dei numeri 0~9 così come visualizzati nel carattere dello stile normale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la larghezza della colonna per l'indice colonna 255
            cells.SetColumnWidth(255, 20.86);

            // Ottieni e visualizza la larghezza della colonna
            double columnWidth = cells.GetColumnWidth(255);
            Console.WriteLine("Column width at index 255: " + columnWidth);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


