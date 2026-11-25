---
title: "Enum CopyFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.CopyFormatType. Rappresenta il tipo di formato di copia durante l'inserimento di righe"
type: docs
url: /it/net/aspose.cells/copyformattype/
---
## CopyFormatType enumeration

Rappresenta il tipo di formato di copia durante l'inserimento di righe.

```csharp
public enum CopyFormatType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| SameAsAbove | `0` | Formato uguale alla riga sopra. |
| SameAsBelow | `1` | Formato uguale alla riga sotto. |
| Clear | `2` | Cancella la formattazione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CopyFormatTypeDemo
    {
        public static void CopyFormatTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // Crea InsertOptions e imposta CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Inserisci una riga nella seconda posizione con il tipo di formato specificato
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Salva la cartella di lavoro
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


