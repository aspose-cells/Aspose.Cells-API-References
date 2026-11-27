---
title: "XmlSaveOptions.XmlSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlSaveOptions konstruktor. Skapar alternativ för att spara xml‑fil"
type: docs
url: /sv/net/aspose.cells/xmlsaveoptions/xmlsaveoptions/
---
## XmlSaveOptions constructor

Skapar alternativ för att spara XML‑fil.

```csharp
public XmlSaveOptions()
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(63);

            // Första demo: Spara som XML med SheetNameAsElementName
            XmlSaveOptions saveOptions1 = new XmlSaveOptions();
            saveOptions1.SheetNameAsElementName = true;
            workbook.Save("output1.xml", saveOptions1);
            
            // Andra demo: Spara som XML med SheetNameAsElementName och DataAsAttribute
            XmlSaveOptions saveOptions2 = new XmlSaveOptions();
            saveOptions2.SheetNameAsElementName = true;
            saveOptions2.DataAsAttribute = true;
            workbook.Save("output2.xml", saveOptions2);

            Console.WriteLine("XML files created successfully.");
        }
    }
}
```

### Se även

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


