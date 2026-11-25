---
title: "Cells.DeleteColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Elimina una colonna"
type: docs
url: /it/net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

Elimina una colonna.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice della colonna da eliminare. |
| updateReference | Booleano | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Inserisci alcuni dati di esempio nelle celle
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }
            
            Console.WriteLine("Before deleting column:");
            PrintCellValues(sheet);
            
            // Elimina la prima colonna e sposta le colonne rimanenti a sinistra
            sheet.Cells.DeleteColumn(0, true);
            
            Console.WriteLine("\nAfter deleting column 0:");
            PrintCellValues(sheet);
            
            // Salva la cartella di lavoro
            workbook.Save("DeleteColumnDemo.xlsx");
        }
        
        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    Console.Write(sheet.Cells[i, j].Value + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumn(int) {#deletecolumn}

Elimina una colonna.

```csharp
public void DeleteColumn(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice della colonna da eliminare. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Inserisci alcuni dati di esempio nelle colonne
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Elimina la colonna all'indice 1 (Colonna B)
            cells.DeleteColumn(1);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Column deleted successfully.");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


