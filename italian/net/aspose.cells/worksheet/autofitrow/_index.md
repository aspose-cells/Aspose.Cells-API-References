---
title: "Worksheet.AutoFitRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Adatta automaticamente l'altezza della riga in un intervallo rettangolare"
type: docs
url: /it/net/aspose.cells/worksheet/autofitrow/
---
## AutoFitRow(int, int, int, int) {#autofitrow_3}

Adatta automaticamente l'altezza della riga in un intervallo rettangolare.

```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale. |
| endRow | Int32 | Indice della riga finale. |
| startColumn | Int32 | Indice della colonna iniziale. |
| endColumn | Int32 | Indice della colonna finale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RowCollection rows = worksheet.Cells.Rows;
            rows[0].Height = 20;
            rows[1].Height = 20;
            // Aggiungi dati di esempio alle celle per dimostrare l'adattamento automatico della riga
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row autofit");
            worksheet.Cells["B1"].PutValue("Additional column with text");
            worksheet.Cells["A2"].PutValue("Shorter text");
            worksheet.Cells["B2"].PutValue("More text");
            
            try
            {
                Console.WriteLine($"Row 1 height before autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height before autofit: {worksheet.Cells.Rows[1].Height}");

                // Chiama AutoFitRow con i parametri: startRow, endRow, startColumn, endColumn
                worksheet.AutoFitRow(0, 1, 0, 1);
                
                Console.WriteLine("AutoFitRow method executed successfully with parameters (0, 1, 0, 1)");
                
                // Mostra l'effetto visualizzando le altezze delle righe
                Console.WriteLine($"Row 1 height after autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height after autofit: {worksheet.Cells.Rows[1].Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitRow method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("AutoFitRowWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int) {#autofitrow}

Adatta automaticamente l'altezza della riga.

```csharp
public void AutoFitRow(int rowIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |

### Osservazioni

AutoFitRow è una funzione imprecisa.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta testo lungo con a capo automatico nella cella A1
            worksheet.Cells["A1"].Value = "LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT";
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Adatta automaticamente la prima riga
            worksheet.AutoFitRow(0);

            // Salva la cartella di lavoro
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int) {#autofitrow_1}

Adatta automaticamente l'altezza della riga.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| lastColumn | Int32 | Indice dell'ultima colonna. |

### Osservazioni

Questo metodo adatta automaticamente una riga in base al contenuto di un intervallo di celle all'interno della riga.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle che influenzeranno l'altezza della riga
            worksheet.Cells["A2"].PutValue("This is a long text that will demonstrate AutoFitRow functionality");
            worksheet.Cells["B2"].PutValue("Additional text in another column");
            
            // Adatta automaticamente la riga (riga 2) tra le colonne 0 e 1 (A a B)
            worksheet.AutoFitRow(1, 0, 1);
            
            // Salva la cartella di lavoro
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}

Adatta automaticamente l'altezza della riga.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |
| firstColumn | Int32 | Indice della prima colonna. |
| lastColumn | Int32 | Indice dell'ultima colonna. |
| opzioni | AutoFitterOptions | Le opzioni dell'auto adattatore |

### Osservazioni

Questo metodo adatta automaticamente una riga in base al contenuto di un intervallo di celle all'interno della riga.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32AutoFitterOptioDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["B1"].PutValue("Another test string in column B");
            
            // Crea AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitMergedCells = true,
                IgnoreHidden = false,
                OnlyAuto = false
            };

            // Ottieni l'altezza originale della riga
            double originalHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"Original row height: {originalHeight}");

            // Adatta automaticamente la prima riga
            worksheet.AutoFitRow(0, 0, 2, options);

            // Ottieni l'altezza della nuova riga
            double newHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"New row height after AutoFit: {newHeight}");

            // Salva la cartella di lavoro
            workbook.Save("AutoFitRowExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


