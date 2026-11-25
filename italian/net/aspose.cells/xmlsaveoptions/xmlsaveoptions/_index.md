---
title: "XmlSaveOptions.XmlSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore XmlSaveOptions. Crea le opzioni per salvare un file xml"
type: docs
url: /it/net/aspose.cells/xmlsaveoptions/xmlsaveoptions/
---
## XmlSaveOptions constructor

Crea le opzioni per salvare il file XML.

```csharp
public XmlSaveOptions()
```

### Esempi

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
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(63);

            // Prima demo: Salva come XML con SheetNameAsElementName
            XmlSaveOptions saveOptions1 = new XmlSaveOptions();
            saveOptions1.SheetNameAsElementName = true;
            workbook.Save("output1.xml", saveOptions1);
            
            // Seconda demo: Salva come XML con SheetNameAsElementName e DataAsAttribute
            XmlSaveOptions saveOptions2 = new XmlSaveOptions();
            saveOptions2.SheetNameAsElementName = true;
            saveOptions2.DataAsAttribute = true;
            workbook.Save("output2.xml", saveOptions2);

            Console.WriteLine("XML files created successfully.");
        }
    }
}
```

### Vedi anche

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


