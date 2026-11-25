---
title: "XmlLoadOptions.IsXmlMap"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlLoadOptions. Indica se mappare xml su Excel. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

Indica se mappare XML in Excel. Il valore predefinito è false.

```csharp
public bool IsXmlMap { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIsXmlMapDemo
    {
        public static void Run()
        {
            // Crea un'istanza di XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Abilita la mappatura XML durante il caricamento del file
            options.IsXmlMap = true;

            // Carica un file XML in un Workbook usando le opzioni specificate
            Workbook workbook = new Workbook("sample.xml", options);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Visualizza alcuni dati dall'XML caricato per dimostrare la mappatura riuscita
            Console.WriteLine("Data from loaded XML:");
            Console.WriteLine(worksheet.Cells["A1"].StringValue);
            Console.WriteLine(worksheet.Cells["A2"].StringValue);

            // Salva la cartella di lavoro in un nuovo file Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


