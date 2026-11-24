---
title: "XmlLoadOptions.ConvertNumericOrDate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlLoadOptions-Eigenschaft. Gibt an, ob der Wert in der XML-Datei in numerisch oder Datum konvertiert wird"
type: docs
url: /de/net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

Gibt an, ob der Wert in der XML‑Datei in numerisch oder Datum konvertiert wird.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            // XML-Ladeoptionen erstellen
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Setzen Sie ConvertNumericOrDate auf true (Standard)
            options.ConvertNumericOrDate = true;
            Workbook wb1 = new Workbook("input.xml", options);
            Cell cell1 = wb1.Worksheets[0].Cells["A1"];
            Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
            
            // Setzen Sie ConvertNumericOrDate auf false
            options.ConvertNumericOrDate = false;
            Workbook wb2 = new Workbook("input.xml", options);
            Cell cell2 = wb2.Worksheets[0].Cells["A1"];
            Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
            
            // Ergebnisse speichern
            wb1.Save("output_with_conversion.xlsx");
            wb2.Save("output_without_conversion.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


