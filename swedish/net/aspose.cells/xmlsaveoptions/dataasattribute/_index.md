---
title: "XmlSaveOptions.DataAsAttribute"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlSaveOptions-egenskap. Anger om data exporteras som attribut för elementet"
type: docs
url: /sv/net/aspose.cells/xmlsaveoptions/dataasattribute/
---
## XmlSaveOptions.DataAsAttribute property

Anger om data exporteras som attribut för elementet.

```csharp
public bool DataAsAttribute { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyDataAsAttributeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Skapa XML-sparalternativ med DataAsAttribute satt till true
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                DataAsAttribute = true,
                SheetNameAsElementName = true
            };

            // Spara med data som attribut
            workbook.Save("DataAsAttribute_True.xml", saveOptions);

            // Ändra för att spara data som element
            saveOptions.DataAsAttribute = false;
            workbook.Save("DataAsAttribute_False.xml", saveOptions);
        }
    }
}
```

### Se även

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


