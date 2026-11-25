---
title: "Enum PaneStateType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.PaneStateType enum. Rappresenta lo stato del riquadro dei fogli"
type: docs
url: /it/net/aspose.cells/panestatetype/
---
## PaneStateType enumeration

Rappresenta lo stato del riquadro del foglio.

```csharp
public enum PaneStateType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Frozen | `0` | I riquadri sono congelati, ma non lo erano prima di essere congelati. |
| FrozenSplit | `1` | I riquadri sono congelati e sono stati divisi prima di essere congelati. |
| Split | `2` | I riquadri sono divisi, ma non congelati. |
| Normal | `3` | I riquadri non sono congelati e non sono divisi. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PaneStateTypeDemo
    {
        public static void PaneStateTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni dati di esempio nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Congela i riquadri nella cella B2
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Verifica lo stato del riquadro
            PaneStateType paneState = worksheet.PaneState;

            // Restituisci lo stato del riquadro
            Console.WriteLine("Current Pane State: " + paneState);

            // Salva la cartella di lavoro
            workbook.Save("PaneStateTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


