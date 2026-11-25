---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlLoadOptions. Indica se ignorare gli attributi dell'elemento radice"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Indica se ignorare gli attributi dell'elemento radice.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento XML e imposta IgnoreRootAttributes
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // Carica il file XML con le opzioni
            Workbook workbook = new Workbook("example.xml", options);

            // Accedi ai dati dall'XML caricato
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // Salva come XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


