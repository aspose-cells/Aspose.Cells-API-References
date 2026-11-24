---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsSaveOptions‑Eigenschaft. Gibt die ODF-Version zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

Liest und setzt die ODF-Version.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // ODS-Speicheroptionen erstellen
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // ODF-Version auf 1.2 festlegen
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Mit angegebener ODF-Version speichern
            workbook.Save("OdfVersion12.ods", saveOptions);

            // Auf ODF-Version 1.3 ändern
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### Siehe auch

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


