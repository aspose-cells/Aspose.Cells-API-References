---
title: "XmlLoadOptions.IsXmlMap"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlLoadOptions-Eigenschaft. Gibt an, ob XML nach Excel abgebildet wird. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

Gibt an, ob XML nach Excel abgebildet wird. Der Standardwert ist false.

```csharp
public bool IsXmlMap { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIsXmlMapDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Aktiviere XML-Mapping beim Laden der Datei
            options.IsXmlMap = true;

            // Lade eine XML-Datei in ein Workbook mit den angegebenen Optionen
            Workbook workbook = new Workbook("sample.xml", options);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Zeige einige Daten aus dem geladenen XML an, um das erfolgreiche Mapping zu demonstrieren
            Console.WriteLine("Data from loaded XML:");
            Console.WriteLine(worksheet.Cells["A1"].StringValue);
            Console.WriteLine(worksheet.Cells["A2"].StringValue);

            // Speichere die Arbeitsmappe in einer neuen Excel-Datei
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


