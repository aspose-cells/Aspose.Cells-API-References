---
title: "XmlSaveOptions.DataAsAttribute"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlSaveOptions. Indica se i dati vengono esportati come attributi dell'elemento"
type: docs
url: /it/net/aspose.cells/xmlsaveoptions/dataasattribute/
---
## XmlSaveOptions.DataAsAttribute property

Indica se esportare i dati come attributi dell'elemento.

```csharp
public bool DataAsAttribute { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyDataAsAttributeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Crea le opzioni di salvataggio XML con DataAsAttribute impostato su true
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                DataAsAttribute = true,
                SheetNameAsElementName = true
            };

            // Salva con i dati come attributi
            workbook.Save("DataAsAttribute_True.xml", saveOptions);

            // Modifica per salvare i dati come elementi
            saveOptions.DataAsAttribute = false;
            workbook.Save("DataAsAttribute_False.xml", saveOptions);
        }
    }
}
```

### Vedi anche

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


