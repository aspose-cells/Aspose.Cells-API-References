---
title: "XmlSaveOptions.HasHeaderRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlSaveOptions. Indica se l'intervallo contiene una riga di intestazione"
type: docs
url: /it/net/aspose.cells/xmlsaveoptions/hasheaderrow/
---
## XmlSaveOptions.HasHeaderRow property

Indica se l'intervallo contiene la riga di intestazione.

```csharp
public bool HasHeaderRow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi la riga di intestazione e i dati
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea le opzioni di salvataggio XML
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.HasHeaderRow = true; // Demonstrate HasHeaderRow property
            saveOptions.SheetNameAsElementName = true;

            // Salva come file XML
            workbook.Save("output.xml", saveOptions);

            Console.WriteLine("XML file saved with HasHeaderRow=true");
        }
    }
}
```

### Vedi anche

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


