---
title: "WorksheetCollection.GetRangeByName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection metodo. Restituisce l'oggetto Range per nome predefinito"
type: docs
url: /it/net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Ottiene l'oggetto Range per nome predefinito.

```csharp
public Range GetRangeByName(string rangeName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeName | String | Nome dell'intervallo. |

### Valore di ritorno

Oggetto Range.

Restituisce null se l'intervallo denominato non esiste.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetRangeByNameWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Crea un intervallo denominato
            worksheet.Cells.CreateRange("A1:B2").Name = "FruitData";
            
            // Ottieni l'intervallo nominato usando GetRangeByName
            Aspose.Cells.Range namedRange = workbook.Worksheets.GetRangeByName("FruitData");
            
            // Visualizza le informazioni dell'intervallo se trovate
            if (namedRange != null)
            {
                Console.WriteLine("Range found: " + namedRange.Address);
                Console.WriteLine("First cell value: " + namedRange[0, 0].StringValue);
            }
            else
            {
                Console.WriteLine("Range not found");
            }
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Restituisce [`Range`](../../range/) per nome predefinito o nome della tabella

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeName | String | Nome dell'intervallo o nome della tabella. |
| currentSheetIndex | Int32 | L'indice del foglio. -1 rappresenta globale. |
| includeTable | Booleano | Indica se controllare tutte le tabelle. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetRangeByNameWithStringInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo denominato
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1", "C3");
            namedRange.Name = "TestRange";
            
            // Aggiungi alcuni dati all'intervallo
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            try
            {
                // Chiama GetRangeByName con i parametri (String, Int32, Boolean)
                Aspose.Cells.Range retrievedRange = workbook.Worksheets.GetRangeByName("TestRange", 0, true);
                
                Console.WriteLine("Method executed successfully with parameters (String, Int32, Boolean)");
                Console.WriteLine($"Retrieved range address: {retrievedRange.Address}");
                Console.WriteLine($"Range contains {retrievedRange.RowCount} rows and {retrievedRange.ColumnCount} columns");
                
                // Visualizza i valori dell'intervallo
                Console.WriteLine("Range values:");
                foreach (Cell cell in retrievedRange)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRangeByName method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("WorksheetCollectionMethodGetRangeByNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


