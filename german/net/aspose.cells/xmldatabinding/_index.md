---
title: "Klasse XmlDataBinding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.XmlDataBinding‑Klasse. Stellt Informationen zur XML‑Datenbindung dar"
type: docs
url: /de/net/aspose.cells/xmldatabinding/
---
## XmlDataBinding class

Stellt Informationen zur XML‑Datenbindung dar.

```csharp
public class XmlDataBinding
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | Liest die Quell‑URL dieser Datenbindung. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellsClassXmlDataBindingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein List‑Objekt, das XML‑Datenbindung verwendet
            ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];

            // Rufe die XML‑Datenbindungsinformationen ab (dies wird typischerweise beim Importieren von XML‑Daten gesetzt)
            XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;

            // Anzeige der URL der XML-Datenquelle (schreibgeschützte Eigenschaft)
            Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);

            // Hinweis: In einem realen Szenario würde die Url beim Importieren von XML-Daten gesetzt werden
            // Zu Demonstrationszwecken zeigen wir, wie man auf die Eigenschaft zugreift

            // Speichere die Arbeitsmappe
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


