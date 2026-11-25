---
title: "Cells.InsertRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento"
type: docs
url: /it/net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | CellArea | Sposta area. |
| shiftNumber | Int32 | Numero di righe o colonne da inserire. |
| shiftType | ShiftType | Opzione sposta celle. |
| updateReference | Booleano | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola alcuni dati di esempio
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);

            // Definisci l'area da inserire (righe 2-3, colonna A)
            CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);

            // Inserisci intervallo spostando le celle a destra e aggiornando i riferimenti
            cells.InsertRange(area, 1, ShiftType.Right, true);

            // Verifica l'operazione controllando i valori
            Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
            Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | CellArea | Sposta area. |
| shiftType | ShiftType | Opzione sposta celle. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Inserisci alcuni dati di esempio
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"R{row}C{col}");
                }
            }

            // Definisci l'area di celle da inserire
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.EndRow = 4;
            area.StartColumn = 1;
            area.EndColumn = 3;

            // Inserisci intervallo e sposta le celle verso il basso
            cells.InsertRange(area, ShiftType.Down);

            // Salva la cartella di lavoro
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

Inserisce un intervallo di celle e sposta le celle secondo l'opzione di spostamento.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| area | CellArea | Sposta area. |
| shiftNumber | Int32 | Numero di righe o colonne da inserire. |
| shiftType | ShiftType | Opzione sposta celle. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Original Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["C1"].PutValue(200);
            
            // Definisci l'area di celle da inserire (cella singola B1)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 1;
            area.EndColumn = 1;
            
            // Inserisci intervallo spostando le celle a destra
            worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
            
            // Salva la cartella di lavoro
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


