---
title: "Enum ShiftType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.ShiftType. Rappresenta le opzioni di spostamento quando si elimina un intervallo di celle"
type: docs
url: /it/net/aspose.cells/shifttype/
---
## ShiftType enumeration

Rappresenta le opzioni di spostamento quando si elimina un intervallo di celle.

```csharp
public enum ShiftType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Down | `0` | Sposta le celle verso il basso. |
| Left | `1` | Sposta le celle verso sinistra. |
| None | `2` | Non spostare le celle. |
| Right | `3` | Sposta le celle verso destra. |
| Up | `4` | Sposta le celle verso l'alto. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ShiftTypeDemo
    {
        public static void ShiftTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Inserisci una nuova riga all'indice 1, spostando le righe esistenti verso il basso
            worksheet.Cells.InsertRows(1, 1, true);

            // Imposta un valore nella riga appena inserita
            worksheet.Cells["A1"].PutValue("New Item");

            // Elimina un intervallo di celle e sposta le celle verso l'alto
            worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);

            // Restituisci i valori rimanenti nella prima colonna
            for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
            {
                Console.WriteLine(worksheet.Cells[row, 0].StringValue);
            }

            // Salva la cartella di lavoro
            workbook.Save("ShiftTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


