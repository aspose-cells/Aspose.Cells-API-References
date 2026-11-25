---
title: "CellArea.CreateCellArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CellArea. Crea un'area cella."
type: docs
url: /it/net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Crea un'area di celle.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | La riga iniziale. |
| startColumn | Int32 | La colonna iniziale. |
| endRow | Int32 | La riga finale. |
| endColumn | Int32 | La colonna finale. |

### Valore di ritorno

Restituisci un [`CellArea`](../).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Popola le celle con dati di esempio
            int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < values.Length; i++)
            {
                cells[i, i / 3].PutValue(values[i]);
            }

            // Crea e configura l'ordinatore dei dati
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;

            // Ordina usando CreateCellArea con parametri Int32
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));

            // Genera i valori ordinati
            Console.WriteLine("Sorted values:");
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine(cells[i, 2 - i / 3].IntValue);
            }
        }
    }
}
```

### Vedi anche

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Crea un'area di celle.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startCellName | String | La cella in alto a sinistra dell'intervallo. |
| endCellName | String | La cella in basso a destra dell'intervallo. |

### Valore di ritorno

Restituisci un [`CellArea`](../).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Popola alcuni dati nella colonna A
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Data {i}");
            }

            // Crea un'area di celle da B1 a B10
            CellArea area = CellArea.CreateCellArea("B1", "B10");
            
            // Inserisci l'intervallo spostando le celle verso il basso
            cells.InsertRange(area, ShiftType.Down);
            
            // Verifica l'operazione controllando i valori delle celle
            Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


