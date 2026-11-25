---
title: "Classe CopyOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CopyOptions. Rappresenta le opzioni di copia"
type: docs
url: /it/net/aspose.cells/copyoptions/
---
## CopyOptions class

Rappresenta le opzioni di copia.

```csharp
public class CopyOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CopyOptions](copyoptions/)() | Costruttore CopyOptions. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | Indica se copiare la larghezza delle colonne in unità di caratteri. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | Se la formula non è valida per la destinazione, copia solo i valori. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | Indica se copiare i nomi. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | Indica se estendere gli intervalli quando si copia l'intervallo a quello adiacente. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | Indica se mantenere le macro; |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | Durante la copia dell'intervallo nello stesso file e se il grafico fa riferimento al foglio di origine, False indica che l'origine dati del grafico copiato non verrà modificata. True indica che l'origine dati del grafico copiato fa riferimento al foglio di destinazione. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli di lavoro durante la copia di un foglio in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. Tuttavia, in alcune situazioni l'utente potrebbe aver bisogno che le formule copiate facciano riferimento a fogli con lo stesso nome nella stessa cartella di lavoro, ad esempio quando quei fogli sono stati copiati prima di questa operazione di copia; in tal caso questa proprietà dovrebbe rimanere impostata su true. |
| [UpdateInvalidReferencesToTargetSheet](../../aspose.cells/copyoptions/updateinvalidreferencestotargetsheet/) { get; set; } | Indica se fare riferimento al foglio di destinazione se il foglio di riferimento non è stato copiato. |

### Esempi

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CopyOptionsDemo
    {
        public static void CopyOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Crea un nuovo workbook in cui copiare i dati
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Crea un oggetto CopyOptions
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // Copia i dati dal worksheet di origine al worksheet di destinazione
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // Salva il workbook di destinazione
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


