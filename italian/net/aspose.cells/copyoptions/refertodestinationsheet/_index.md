---
title: "CopyOptions.ReferToDestinationSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CopyOptions. Quando si copia l'intervallo nello stesso file e il grafico fa riferimento al foglio di origine, False indica che la fonte dati del grafico copiato non verrà modificata. True indica che la fonte dati del grafico copiato fa riferimento al foglio di destinazione."
type: docs
url: /it/net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

Durante la copia dell'intervallo nello stesso file e se il grafico fa riferimento al foglio di origine, False indica che l'origine dati del grafico copiato non verrà modificata. True indica che l'origine dati del grafico copiato fa riferimento al foglio di destinazione.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Osservazioni

Il valore predefinito è false, funziona come MS Excel. Per esempio: se si copia un grafico con la fonte dati \"sheet1!A1:B10\" dal foglio di lavoro \"sheet1\" a un altro foglio di lavoro \"sheet2\", la fonte dati verrà modificata in \"sheet2!A1:B10\".

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToDestinationSheetDemo
    {
        public static void Run()
        {
            // Crea la cartella di lavoro di origine con dati di esempio
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B1"].PutValue(100);
            sourceSheet.Cells["A2"].PutValue("=SUM(B1)");

            // Crea la cartella di lavoro di destinazione
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");

            // Imposta le opzioni di copia con ReferToDestinationSheet
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            // Copia il foglio di lavoro con le opzioni
            destSheet.Copy(sourceSheet, copyOptions);

            // Salva il risultato
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


