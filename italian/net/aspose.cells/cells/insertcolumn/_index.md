---
title: "Cells.InsertColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Inserisce una nuova colonna nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

Inserisce una nuova colonna nel foglio di lavoro.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice colonna. |
| updateReference | Booleano | Indica se i riferimenti in altri fogli di lavoro verranno aggiornati. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio nella colonna 0
            Cells cells = sheet.Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue($"Original {i}");
            }

            // Inserisci una nuova colonna all'indice 1 e sposta le colonne a destra
            cells.InsertColumn(1, true);

            // Copia i dati dalla colonna 0 alla nuova colonna 1
            cells.CopyColumn(cells, 0, 1);

            // Salva la cartella di lavoro
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

Inserisce una nuova colonna nel foglio di lavoro.

```csharp
public void InsertColumn(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice colonna. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ottieni la raccolta di celle
            Cells cells = sheet.Cells;
            
            // Inserisci dati nelle celle per dimostrazione
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Inserisci una nuova colonna all'indice 1 (diventerà la nuova colonna B)
            cells.InsertColumn(1);
            
            // Verifica inserendo dati nella nuova colonna
            cells["B1"].PutValue("New Column");
            
            // Salva la cartella di lavoro
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


