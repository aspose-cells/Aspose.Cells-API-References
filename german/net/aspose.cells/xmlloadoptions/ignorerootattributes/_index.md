---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlLoadOptions-Eigenschaft. Gibt an, ob Attribute des Root-Elements ignoriert werden"
type: docs
url: /de/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Gibt an, ob Attribute des Root-Elements ignoriert werden.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // Erstelle XML-Ladeoptionen und setze IgnoreRootAttributes
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // Lade XML-Datei mit den Optionen
            Workbook workbook = new Workbook("example.xml", options);

            // Greife auf Daten aus dem geladenen XML zu
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // Als XLSX speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


