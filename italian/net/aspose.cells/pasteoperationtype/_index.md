---
title: "Enum PasteOperationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.PasteOperationType. Rappresenta il tipo di operazione durante l'incollaggio di un intervallo"
type: docs
url: /it/net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Rappresenta il tipo di operazione durante l'incollaggio di un intervallo.

```csharp
public enum PasteOperationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna operazione. |
| Add | `1` | Aggiungi |
| Subtract | `2` | Sottrai |
| Multiply | `3` | Moltiplica |
| Divide | `4` | Dividi |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPasteOperationTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(30);
            
            // Crea opzioni di incollaggio con PasteOperationType.None
            var pasteOptions = new PasteOptions()
            {
                PasteType = PasteType.Values,
                OperationType = PasteOperationType.None,
                SkipBlanks = false,
                Transpose = false
            };

            // Crea un intervallo e copia con le opzioni di incollaggio
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
            Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
            sourceRange.Copy(destRange, pasteOptions);

            // Salva la cartella di lavoro
            workbook.Save("PasteOperationTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


