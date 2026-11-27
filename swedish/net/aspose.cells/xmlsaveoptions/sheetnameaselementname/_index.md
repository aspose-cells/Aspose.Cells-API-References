---
title: "XmlSaveOptions.SheetNameAsElementName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlSaveOptions egenskap. Anger om bladnamn exporteras som elementets namn"
type: docs
url: /sv/net/aspose.cells/xmlsaveoptions/sheetnameaselementname/
---
## XmlSaveOptions.SheetNameAsElementName property

Anger om bladets namn exporteras som elementets namn.

```csharp
public bool SheetNameAsElementName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertySheetNameAsElementNameDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "EmployeeData";
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Spara med SheetNameAsElementName = true (standard)
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            workbook.Save("output_with_sheetname.xml", saveOptions);

            // Spara med SheetNameAsElementName = false
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output_without_sheetname.xml", saveOptions);

            Console.WriteLine("XML files created successfully with different SheetNameAsElementName settings.");
        }
    }
}
```

### Se även

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


