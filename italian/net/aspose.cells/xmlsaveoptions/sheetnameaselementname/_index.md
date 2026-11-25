---
title: "XmlSaveOptions.SheetNameAsElementName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlSaveOptions. Indica se esportare il nome dei fogli come nome dell'elemento"
type: docs
url: /it/net/aspose.cells/xmlsaveoptions/sheetnameaselementname/
---
## XmlSaveOptions.SheetNameAsElementName property

Indica se esportare il nome del foglio come nome dell'elemento.

```csharp
public bool SheetNameAsElementName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertySheetNameAsElementNameDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "EmployeeData";
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Salva con SheetNameAsElementName = true (predefinito)
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            workbook.Save("output_with_sheetname.xml", saveOptions);

            // Salva con SheetNameAsElementName = false
            saveOptions.SheetNameAsElementName = false;
            workbook.Save("output_without_sheetname.xml", saveOptions);

            Console.WriteLine("XML files created successfully with different SheetNameAsElementName settings.");
        }
    }
}
```

### Vedi anche

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


