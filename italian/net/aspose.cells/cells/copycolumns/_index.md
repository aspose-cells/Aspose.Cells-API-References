---
title: "Cells.CopyColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Copia dati e formati di un'intera colonna"
type: docs
url: /it/net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

Copia i dati e i formati di un'intera colonna.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | Celle | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceColumnIndex | Int32 | Indice della colonna di origine. |
| destinationColumnIndex | Int32 | Indice della colonna di destinazione. |
| columnNumber | Int32 | Il numero della colonna copiata. |
| pasteOptions | PasteOptions | le opzioni di incolla. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // Crea un altro workbook come destinazione
            Workbook destWorkbook = new Workbook();
            Worksheet destWorksheet = destWorkbook.Worksheets[0];

            // Copia le colonne solo con la formattazione
            try
            {
                destWorksheet.Cells.CopyColumns(
                    worksheet.Cells, 
                    0, // source column index
                    0, // destination column index
                    2, // column count (copy 2 columns)
                    new PasteOptions() { PasteType = PasteType.Formats });
                
                Console.WriteLine("Columns copied successfully with formatting only.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error copying columns: " + ex.Message);
            }

            // Salva la cartella di lavoro
            workbook.Save("CopyColumnsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int) {#copycolumns}

Copia i dati e i formati di intere colonne.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | Celle | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceColumnIndex | Int32 | Indice della colonna di origine. |
| destinationColumnIndex | Int32 | Indice della colonna di destinazione. |
| columnNumber | Int32 | Il numero della colonna copiata. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio alle colonne
            cells["A1"].PutValue("Source1");
            cells["B1"].PutValue("Source2");
            cells["C1"].PutValue("Source3");
            cells["D1"].PutValue("Source4");
            cells["E1"].PutValue("Source5");

            // Copia le colonne dall'indice colonna 1 (B) all'indice colonna 3 (D), copia 1 colonna
            cells.CopyColumns(cells, 1, 3, 1);

            // Salva la cartella di lavoro
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

Copia i dati e i formati di tutte le colonne.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceCells | Celle | L'oggetto Source Cells contiene dati e formati da copiare. |
| sourceColumnIndex | Int32 | Indice della colonna di origine. |
| sourceTotalColumns | Int32 | Il numero delle colonne di origine. |
| destinationColumnIndex | Int32 | Indice della colonna di destinazione. |
| destinationTotalColumns | Int32 | Il numero delle colonne di destinazione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola le colonne di origine (colonne 0 e 1)
            cells[0, 0].Value = "Header 1";
            cells[0, 1].Value = "Header 2";
            for (int row = 1; row <= 4; row++)
            {
                cells[row, 0].Value = row * 100;
                cells[row, 1].Value = row * 200;
            }

            try
            {
                // Copia 2 colonne dall'indice 0 all'indice di destinazione 3, inserendo 2 colonne
                cells.CopyColumns(cells, 0, 2, 3, 2);
                
                Console.WriteLine("Copied 2 source columns to destination position successfully");
                
                // Verifica la copia controllando le colonne di destinazione (3 e 4)
                Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
                Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


