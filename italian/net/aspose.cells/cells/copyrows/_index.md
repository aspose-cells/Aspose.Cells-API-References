---
title: "Cells.CopyRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Copia dati e formati di alcune righe intere"
type: docs
url: /it/net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Copia i dati e i formati di alcune intere righe.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | Celle | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceRowIndex | Int32 | Indice della riga di origine. |
| destinationRowIndex | Int32 | Indice della riga di destinazione. |
| rowNumber | Int32 | Il numero della riga copiata. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook destinationWorkbook = new Workbook();
            Workbook sourceWorkbook = new Workbook();

            // Aggiungi alcuni dati di esempio alla cartella di lavoro di origine
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data 1");
            sourceSheet.Cells["A2"].PutValue("Source Data 2");
            sourceSheet.Cells["A3"].PutValue("Source Data 3");

            // Ottieni le celle da entrambe le cartelle di lavoro
            Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
            Cells sourceCells = sourceSheet.Cells;

            // Copia tutte le righe dalla sorgente alla destinazione iniziando dalla riga 0 nella destinazione
            destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);

            // Salva il risultato
            destinationWorkbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Copia i dati e i formati di alcune intere righe.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, 
    CopyOptions copyOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | Celle | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceRowIndex | Int32 | Indice della riga di origine. |
| destinationRowIndex | Int32 | Indice della riga di destinazione. |
| rowNumber | Int32 | Il numero della riga copiata. |
| copyOptions | CopyOptions | Le opzioni di copia. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio e collegamenti ipertestuali
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Inserisci una riga vuota nella riga 5
            worksheet.Cells.InsertRows(5, 1);

            // Copia la riga 4 nella riga 5 senza CopyOptions
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
            Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);

            // Reimposta il foglio di lavoro
            worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
            worksheet.Hyperlinks.Clear();
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Inserisci nuovamente una riga vuota nella riga 5
            worksheet.Cells.InsertRows(5, 1);

            // Copia la riga 4 nella riga 5 con CopyOptions
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
            Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Copia i dati e i formati di alcune intere righe.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells0 | Celle | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceRowIndex | Int32 | Indice della riga di origine. |
| destinationRowIndex | Int32 | Indice della riga di destinazione. |
| rowNumber | Int32 | Il numero della riga copiata. |
| copyOptions | CopyOptions | Le opzioni di copia. |
| pasteOptions | PasteOptions | le opzioni di incolla. |

### Vedi anche

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


