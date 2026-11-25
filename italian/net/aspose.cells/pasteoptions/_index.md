---
title: "Classe PasteOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.PasteOptions. Rappresenta le opzioni di incolla speciale"
type: docs
url: /it/net/aspose.cells/pasteoptions/
---
## PasteOptions class

Rappresenta le opzioni di incolla speciale.

```csharp
public class PasteOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PasteOptions](pasteoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | Ignora i collegamenti al file originale. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | Mantiene le tabelle nell'intervallo di destinazione. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | True indica che vengono copiate solo le celle visibili. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | Ottiene e imposta il tipo di operazione durante l'incollaggio dell'intervallo. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | Il tipo di incolla speciale. |
| [ShiftFormulasOfShapes](../../aspose.cells/pasteoptions/shiftformulasofshapes/) { get; set; } | Indica se spostare le formule delle forme durante la copia degli intervalli. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | Indica se saltare le celle vuote. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | True per trasporre righe e colonne quando l'intervallo è incollato. Il valore predefinito è False. |

### Esempi

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsDemo
    {
        public static void PasteOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al primo foglio di lavoro
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Crea un altro foglio di lavoro
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");

            // Definisci l'intervallo di origine
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");

            // Definisci l'intervallo di destinazione
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");

            // Crea l'oggetto PasteOptions
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // Copia l'intervallo con le opzioni di incolla specificate
            destRange.Copy(sourceRange, pasteOptions);

            // Salva la cartella di lavoro
            workbook.Save("PasteOptionsExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


