---
title: "XmlLoadOptions.ConvertNumericOrDate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlLoadOptions. Indica se convertire il valore nel file xml in numerico o data"
type: docs
url: /it/net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

Indica se convertire il valore nel file XML in numerico o data.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento XML
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Imposta ConvertNumericOrDate su true (predefinito)
            options.ConvertNumericOrDate = true;
            Workbook wb1 = new Workbook("input.xml", options);
            Cell cell1 = wb1.Worksheets[0].Cells["A1"];
            Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
            
            // Imposta ConvertNumericOrDate su false
            options.ConvertNumericOrDate = false;
            Workbook wb2 = new Workbook("input.xml", options);
            Cell cell2 = wb2.Worksheets[0].Cells["A1"];
            Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
            
            // Salva i risultati
            wb1.Save("output_with_conversion.xlsx");
            wb2.Save("output_without_conversion.xlsx");
        }
    }
}
```

### Vedi anche

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


