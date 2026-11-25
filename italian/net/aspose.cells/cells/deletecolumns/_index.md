---
title: "Cells.DeleteColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Elimina diverse colonne"
type: docs
url: /it/net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

Elimina diverse colonne.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice della prima colonna da eliminare. |
| totalColumns | Int32 | Numero di colonne da eliminare. |
| updateReference | Booleano | Indica se aggiornare i riferimenti in altri fogli di lavoro. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Aggiungi una formula che fa riferimento a queste colonne
            worksheet.Cells["D1"].Formula = "=SUM(A2:C2)";

            Console.WriteLine("Before deleting columns:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1: " + worksheet.Cells["C1"].Value);
            Console.WriteLine("D1 formula: " + worksheet.Cells["D1"].Formula);

            // Elimina la colonna B (indice 1) e sposta le colonne rimanenti a sinistra
            worksheet.Cells.DeleteColumns(1, 1, true);

            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1 formula: " + worksheet.Cells["C1"].Formula);
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

Elimina diverse colonne.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice della prima colonna da eliminare. |
| totalColumns | Int32 | Numero di colonne da eliminare. |
| opzioni | DeleteOptions | Opzioni per l'operazione di eliminazione |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola dati di esempio nelle colonne A-E
            for (int col = 0; col < 5; col++)
            {
                worksheet.Cells[0, col].Value = $"Column {(char)('A' + col)}";
                worksheet.Cells[1, col].Value = $"Data{col + 1}";
            }

            // Crea DeleteOptions e configura le impostazioni
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Update references in other cells
            };

            try
            {
                // Elimina 2 colonne a partire dalla colonna B (indice 1)
                worksheet.Cells.DeleteColumns(1, 2, options);
                
                Console.WriteLine("Deleted columns B and C successfully");
                
                // Visualizza i dati rimanenti nella colonna B (colonna D originale)
                Console.WriteLine($"New column B value: {worksheet.Cells[1, 1].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteColumns: {ex.Message}");
            }
            
            // Salva la cartella di lavoro modificata
            workbook.Save("DeleteColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


