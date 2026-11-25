---
title: "Cells.ClearFormats"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Cancella la formattazione di un intervallo"
type: docs
url: /it/net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Cancella la formattazione di un range.

```csharp
public void ClearFormats(CellArea range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | CellArea | Intervallo da cancellare. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearFormatsWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea dati di esempio con formattazione
            CellArea formatArea = new CellArea();
            formatArea.StartRow = 0;
            formatArea.StartColumn = 0;
            formatArea.EndRow = 2;
            formatArea.EndColumn = 2;

            // Applica formattazione alle celle
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            
            for (int row = formatArea.StartRow; row <= formatArea.EndRow; row++)
            {
                for (int col = formatArea.StartColumn; col <= formatArea.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Formatted {row},{col}");
                    cells[row, col].SetStyle(style);
                }
            }

            // Definisci l'area da cancellare
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 1;
            clearArea.StartColumn = 1;
            clearArea.EndRow = 1;
            clearArea.EndColumn = 1;

            try
            {
                // Cancella le formattazioni dalla cella centrale
                cells.ClearFormats(clearArea);
                Console.WriteLine($"Cleared formats in area: Row {clearArea.StartRow}-{clearArea.EndRow}, Column {clearArea.StartColumn}-{clearArea.EndColumn}");
                
                // Aggiorna il valore della cella cancellata per mostrare l'effetto
                cells[1, 1].PutValue("Cleared Format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormats: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("CellsMethodClearFormatsWithCellAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearFormats(int, int, int, int) {#clearformats_1}

Cancella la formattazione di un range.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale. |
| startColumn | Int32 | Indice della colonna iniziale. |
| endRow | Int32 | Indice della riga finale. |
| endColumn | Int32 | Indice della colonna finale. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearFormatsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Applica stili a alcune celle
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            cells[0, 0].SetStyle(style);
            cells[0, 10].SetStyle(style);
            cells[10, 0].SetStyle(style);
            cells[10, 10].SetStyle(style);

            // Cancella le formattazioni da un intervallo specifico (righe 5-15, colonne 5-15)
            cells.ClearFormats(5, 5, 15, 15);

            // Salva la cartella di lavoro
            workbook.Save("ClearedFormats.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


