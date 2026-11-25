---
title: "WorksheetCollection.AddCopy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Aggiunge un foglio di lavoro alla collezione e copia i dati da un foglio di lavoro esistente"
type: docs
url: /it/net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Aggiunge un foglio di lavoro alla collezione e copia i dati da un foglio di lavoro esistente.

```csharp
public int AddCopy(string sheetName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | String | Nome del foglio di lavoro di origine. |

### Valore di ritorno

[`Worksheet`](../../worksheet/) object index.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| [CellsException](../../cellsexception/) | Specifica un nome di foglio di lavoro non valido. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro chiamato "Original" alla cartella di lavoro
            Worksheet originalSheet = workbook.Worksheets.Add("Original");
            
            // Aggiungi alcuni dati al foglio di lavoro originale
            originalSheet.Cells["A1"].PutValue("This is the original sheet");
            
            // Crea una copia del foglio di lavoro "Original"
            int copiedIndex = workbook.Worksheets.AddCopy("Original");
            Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
            copiedSheet.Name = "CopiedSheet";
            
            // Modifica il foglio copiato per dimostrare che è una copia separata
            copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetCopyDemo.xlsx");
            
            Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Aggiunge un foglio di lavoro alla collezione e copia i dati da un foglio di lavoro esistente.

```csharp
public int AddCopy(int sheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | Indice del foglio di lavoro di origine. |

### Valore di ritorno

[`Worksheet`](../../worksheet/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Worksheet");
            
            // Aggiungi una copia del primo foglio di lavoro
            workbook.Worksheets.AddCopy(0);
            
            // Verifica che la copia sia stata creata
            Worksheet copiedWorksheet = workbook.Worksheets[1];
            copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Copia un gruppo di fogli di lavoro.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origine | Worksheet[] | I fogli di lavoro di origine. |
| destSheetNames | String[] | I nomi dei fogli copiati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro di esempio
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Popola alcuni dati nei fogli di lavoro
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");

            // Prepara l'array dei fogli di lavoro di origine
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet2"],
                workbook.Worksheets["Sheet3"]
            };

            // Prepara l'array dei nomi dei fogli di destinazione
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet2",
                "CopyOfSheet3"
            };

            try
            {
                // Chiama il metodo AddCopy con i parametri (Worksheet[], String[])
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // Verifica che le copie siano state create
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


