---
title: "Enum MergeEmptyTdType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.MergeEmptyTdType. Rappresenta il tipo di unione per un elemento TD vuoto durante l'esportazione di un file in HTML"
type: docs
url: /it/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

Rappresenta il tipo di unione per un elemento TD vuoto durante l'esportazione di un file in HTML.

```csharp
public enum MergeEmptyTdType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Visualizza come MS Excel. |
| None | `1` | Gli elementi TD vuoti non verranno uniti durante l'esportazione del file in HTML. Questo genererà un file HTML significativamente più grande. |
| MergeForcely | `2` | Unione forzata degli elementi TD vuoti durante l'esportazione del file in HTML. La dimensione del file HTML sarà ridotta significativamente impostando il valore su true. Se desideri importare il file HTML in Excel o esportare linee di griglia perfette quando salvi il file in HTML, mantieni il valore predefinito. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // Crea HtmlSaveOptions e imposta la proprietà MergeEmptyTdType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // Salva la cartella di lavoro in formato HTML
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


