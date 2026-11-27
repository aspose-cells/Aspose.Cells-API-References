---
title: "XmlSaveOptions.ExportArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlSaveOptions-egenskap. Hämtar eller anger exportområdet"
type: docs
url: /sv/net/aspose.cells/xmlsaveoptions/exportarea/
---
## XmlSaveOptions.ExportArea property

Hämtar eller anger exportintervallet.

```csharp
public CellArea ExportArea { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa XmlSaveOptions och ange ExportArea
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Spara endast det angivna området till XML
            workbook.Save("ExportAreaDemo.xml", saveOptions);
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


