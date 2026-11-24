---
title: "XmlSaveOptions.ExportArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlSaveOptions-Eigenschaft. Liest oder setzt den Exportbereich."
type: docs
url: /de/net/aspose.cells/xmlsaveoptions/exportarea/
---
## XmlSaveOptions.ExportArea property

Liest oder setzt den Exportbereich.

```csharp
public CellArea ExportArea { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten im Arbeitsblatt ausfüllen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // XmlSaveOptions erstellen und ExportArea festlegen
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Nur den angegebenen Bereich als XML speichern
            workbook.Save("ExportAreaDemo.xml", saveOptions);
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


