---
title: "Enum GridlineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridlineType enum. Enumera i tipi di linee della griglia"
type: docs
url: /it/net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

Enumera il tipo di linea della griglia.

```csharp
public enum GridlineType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Dotted | `0` | Rappresenta una linea tratteggiata. |
| Hair | `1` | Rappresenta una linea sottile. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGridlineTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea le opzioni di salvataggio e imposta il tipo di linea della griglia
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.GridlineType = GridlineType.Dotted;
            
            // Aggiungi alcuni dati di esempio per vedere le linee della griglia
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            // Salva la cartella di lavoro con le opzioni di salvataggio
            workbook.Save("GridlineTypeDemo.docx", saveOptions);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


