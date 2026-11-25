---
title: "Cells.ImportObjectArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa un array di dati in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/importobjectarray/
---
## ImportObjectArray(object[], int, int, bool) {#importobjectarray}

Importa un array di dati in un foglio di lavoro.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objArray | Object[] | Array di dati. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| isVertical | Booleano | Specifica se importare i dati verticalmente o orizzontalmente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara un array di oggetti con dati di esempio
            object[] dataArray = new object[] { "Product", "Price", "Stock", "Discontinued", 150.5, 75, false };

            try
            {
                // Importa l'array di oggetti nel foglio di lavoro a partire dalla cella B3 (riga 2, colonna 1), orizzontalmente
                worksheet.Cells.ImportObjectArray(dataArray, 2, 1, false);

                Console.WriteLine("Object array imported successfully to cells B3:F3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Salva la cartella di lavoro per dimostrare l'output
            workbook.Save("CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportObjectArray(object[], int, int, bool, int) {#importobjectarray_1}

Importa un array di dati in un foglio di lavoro.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical, 
    int skip)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objArray | Object[] | Array di dati. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| isVertical | Booleano | Specifica se importare i dati verticalmente o orizzontalmente. |
| salta | Int32 | Numero di righe o colonne saltate. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Prepara i dati per i parametri di ImportObjectArray: (Object[], Int32, Int32, Boolean, Int32)
            object[] data = new object[]
            {
                "Name",
                "Age",
                "Date",
                "John Doe",
                30,
                new DateTime(2023, 10, 15),
                "Jane Smith",
                28,
                new DateTime(2023, 10, 16)
            };

            try
            {
                // Chiama ImportObjectArray con i parametri: (array di dati, riga iniziale 0, colonna iniziale 0, importazione orizzontale, salta 1 colonna tra le voci)
                worksheet.Cells.ImportObjectArray(data, 0, 0, false, 1);
                
                Console.WriteLine("Imported object array with parameters (Object[], 0, 0, false, 1) successfully.");
                
                // Dimostrare l'effetto: i dati saranno inseriti nelle celle A1, C1, E1, A2, C2, E2, ecc. con colonne saltate
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportObjectArray: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


