---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsSaveOptions. Ottiene e imposta la versione ODF"
type: docs
url: /it/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

Ottiene e imposta la versione ODF.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyOdfStrictVersionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // Crea le opzioni di salvataggio ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // Imposta la versione ODF a 1.2
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Salva con la versione ODF specificata
            workbook.Save("OdfVersion12.ods", saveOptions);

            // Passa alla versione ODF 1.3
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### Vedi anche

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


