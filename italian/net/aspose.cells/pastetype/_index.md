---
title: "Enum PasteType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.PasteType. Rappresenta il tipo di incolla speciale"
type: docs
url: /it/net/aspose.cells/pastetype/
---
## PasteType enumeration

Rappresenta il tipo di incolla speciale.

```csharp
public enum PasteType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| All | `0` | Copia tutti i dati dell'intervallo. |
| Default | `1` | Funziona come il comportamento "All" di MS Excel. |
| AllExceptBorders | `2` | Copia tutti i dati dell'intervallo senza l'intervallo. |
| DefaultExceptBorders | `3` | Funziona come il comportamento "All except borders" di MS Excel. |
| ColumnWidths | `4` | Copia solo le larghezze dell'intervallo. |
| RowHeights | `5` | Copia solo le altezze dell'intervallo. |
| Comments | `6` | Copia solo i commenti nell'intervallo. |
| Formats | `7` | Copia solo i formati nell'intervallo. |
| Formulas | `8` | Copia solo le formule nell'intervallo. |
| FormulasAndNumberFormats | `9` | Copia solo le formule e i formati numerici nell'intervallo. |
| Validation | `10` | Copia solo le convalide nell'intervallo. |
| Values | `11` | Copia solo i valori nell'intervallo. |
| ValuesAndFormats | `12` | Copia solo i valori e i formati nell'intervallo. |
| ValuesAndNumberFormats | `13` | Copia solo i valori e i formati numerici nell'intervallo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Definisci l'intervallo di origine
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // Definisci l'intervallo di destinazione
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // Crea PasteOptions e imposta PasteType
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // Copia l'intervallo di origine nell'intervallo di destinazione con le opzioni di incolla specificate
            destinationRange.Copy(sourceRange, pasteOptions);

            // Salva la cartella di lavoro
            workbook.Save("PasteTypeExample.xlsx");

            // Restituisci i risultati
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


