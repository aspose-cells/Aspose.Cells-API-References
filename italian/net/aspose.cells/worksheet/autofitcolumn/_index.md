---
title: "Worksheet.AutoFitColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Adatta automaticamente la larghezza della colonna"
type: docs
url: /it/net/aspose.cells/worksheet/autofitcolumn/
---
## AutoFitColumn(int, int, int) {#autofitcolumn_1}

Adatta automaticamente la larghezza della colonna.

```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice colonna. |
| firstRow | Int32 | Indice della prima riga. |
| lastRow | Int32 | Indice dell'ultima riga. |

### Osservazioni

Questo metodo adatta automaticamente una riga in base al contenuto di un intervallo di celle all'interno della riga.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola le celle con dati di esempio che richiederanno la regolazione della larghezza della colonna
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["A2"].PutValue("This is a much longer piece of text that will require column width adjustment");
            worksheet.Cells["A3"].PutValue("Another long text entry to demonstrate AutoFitColumn");
            
            try
            {

                Console.WriteLine($"Column width before: {worksheet.Cells.GetColumnWidth(0)}");
                // Chiama AutoFitColumn sulla colonna A (indice 0) per le righe da 0 a 2 (basato su zero)
                worksheet.AutoFitColumn(0, 0, 2);
                
                Console.WriteLine("AutoFitColumn method executed successfully on column A for rows 1-3");
                
                // Mostra l'effetto visualizzando la larghezza della colonna prima e dopo
                Console.WriteLine($"Column width after: {worksheet.Cells.GetColumnWidth(0)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumn method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("AutoFitColumnWithInt32Int32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumn(int) {#autofitcolumn}

Adatta automaticamente la larghezza della colonna.

```csharp
public void AutoFitColumn(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice colonna. |

### Osservazioni

AutoFitColumn è una funzione imprecisa.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle nella colonna 4 (indice basato su 0)
            worksheet.Cells["D1"].PutValue("This is a test");
            worksheet.Cells["D2"].PutValue("AutoFitColumn demonstration");
            worksheet.Cells["D3"].PutValue("Aspose.Cells for .NET");
            
            // Adatta automaticamente la colonna 4 (indice basato su 0)
            worksheet.AutoFitColumn(3);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


