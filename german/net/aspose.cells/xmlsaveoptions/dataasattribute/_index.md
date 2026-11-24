---
title: "XmlSaveOptions.DataAsAttribute"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlSaveOptions-Eigenschaft. Gibt an, ob Daten als Attribute des Elements exportiert werden"
type: docs
url: /de/net/aspose.cells/xmlsaveoptions/dataasattribute/
---
## XmlSaveOptions.DataAsAttribute property

Gibt an, ob Daten als Attribute des Elements exportiert werden.

```csharp
public bool DataAsAttribute { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyDataAsAttributeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // XML-Speicheroptionen erstellen, wobei DataAsAttribute auf true gesetzt ist
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                DataAsAttribute = true,
                SheetNameAsElementName = true
            };

            // Speichern mit Daten als Attribute
            workbook.Save("DataAsAttribute_True.xml", saveOptions);

            // Ändern, um Daten als Elemente zu speichern
            saveOptions.DataAsAttribute = false;
            workbook.Save("DataAsAttribute_False.xml", saveOptions);
        }
    }
}
```

### Siehe auch

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


