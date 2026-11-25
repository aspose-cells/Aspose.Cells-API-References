---
title: "Enum OoxmlCompressionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.OoxmlCompressionType. Il tipo di compressione Ooxml"
type: docs
url: /it/net/aspose.cells/ooxmlcompressiontype/
---
## OoxmlCompressionType enumeration

Il tipo di compressione Ooxml

```csharp
public enum OoxmlCompressionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Level1 | `1` | La compressione più veloce ma meno efficace. |
| Level2 | `2` | Un po' più lenta, ma migliore, rispetto al livello 1. |
| Level3 | `3` | Un po' più lenta, ma migliore, rispetto al livello 2. |
| Level4 | `4` | Un po' più lenta, ma migliore, rispetto al livello 3. |
| Level5 | `5` | Un po' più lenta rispetto al livello 4, ma con una compressione migliore. |
| Level6 | `6` | Un buon equilibrio tra velocità ed efficienza di compressione. |
| Level7 | `7` | Compressione piuttosto buona! |
| Level8 | `8` | Compressione migliore rispetto al Level7! |
| Level9 | `9` | La compressione "migliore", dove migliore significa la massima riduzione della dimensione del flusso di dati in ingresso. Questa è anche la compressione più lenta. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlCompressionTypeDemo
    {
        public static void OoxmlCompressionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Crea OoxmlSaveOptions e imposta il tipo di compressione
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // Salva la cartella di lavoro con il tipo di compressione specificato
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


