---
title: "XmlSaveOptions.SheetNameAsElementName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlSaveOptions-Eigenschaft. Gibt an, ob der Blattname als Name des Elements exportiert wird"
type: docs
url: /de/net/aspose.cells/xmlsaveoptions/sheetnameaselementname/
---
## XmlSaveOptions.SheetNameAsElementName property

Gibt an, ob der Name des Arbeitsblatts als Name des Elements exportiert wird.

```csharp
public bool SheetNameAsElementName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertySheetNameAsElementNameDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispiel-Arbeitsbuch mit Daten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "EmployeeData";
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Speichern mit SheetNameAsElementName = true (Standard)
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            workbook.Save("output_with_sheetname.xml", saveOptions);

            // Speichern mit SheetNameAsElementName = false
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output_without_sheetname.xml", saveOptions);

            Console.WriteLine("XML files created successfully with different SheetNameAsElementName settings.");
        }
    }
}
```

### Siehe auch

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


