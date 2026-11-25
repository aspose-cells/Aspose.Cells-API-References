---
title: "Enum AutoFillType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.AutoFillType enum. Rappresenta il tipo di riempimento automatico"
type: docs
url: /it/net/aspose.cells/autofilltype/
---
## AutoFillType enumeration

Rappresenta il tipo di riempimento automatico.

```csharp
public enum AutoFillType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Copy | `1` | Copia il valore e il formato dell'area di origine nell'area di destinazione |
| Default | `0` | Riempie automaticamente l'area di destinazione con il valore e il formato. |
| Formats | `3` | Copia solo il formato dell'area di origine nell'area di destinazione. |
| Series | `2` | Estende il valore nell'area di origine all'area di destinazione sotto forma di serie e copia il formato nell'area di destinazione. |
| Values | `4` | Copia solo il valore dell'area di origine nell'area di destinazione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFillTypeDemo
    {
        public static void AutoFillTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo (A1:A10) e riempilo con alcuni valori
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
            for (int i = 0; i < 10; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            // Crea un intervallo di destinazione (B1:B10)
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");

            //Errore di tipo Serie, il ticket è stato creato
            // Usa il metodo AutoFill con AutoFillType.Series per riempire l'intervallo di destinazione
            //sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Usa il metodo AutoFill con AutoFillType.Copy per riempire l'intervallo di destinazione
            sourceRange.AutoFill(targetRange, AutoFillType.Copy);
            // Salva la cartella di lavoro
            workbook.Save("AutoFillTypeExample.xlsx");
            workbook.Save("AutoFillTypeExample.pdf");
        }
    }

}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


