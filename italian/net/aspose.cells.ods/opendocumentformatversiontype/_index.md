---
title: "Enum OpenDocumentFormatVersionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType enum. Tipo di versione del formato Open Document"
type: docs
url: /it/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Tipo di versione del formato Open Document.

```csharp
public enum OpenDocumentFormatVersionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna restrizione. |
| Odf11 | `1` | Versione ODF 1.1 |
| Odf12 | `2` | Versione ODF 1.2 |
| Odf13 | `3` | Versione ODF 1.3 |
| Odf14 | `4` | Versione ODF 1.4 |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OpenDocumentFormatVersionTypeDemo
    {
        public static void OpenDocumentFormatVersionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Crea OdsSaveOptions e imposta la versione ODF
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Salva la cartella di lavoro in formato ODS con la versione ODF specificata
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


