---
title: "XmlLoadOptions.XmlLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlLoadOptions-Konstruktor. Stellt die Optionen für das Laden einer XML-Datei dar"
type: docs
url: /de/net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Stellt die Optionen zum Laden einer XML‑Datei dar.

```csharp
public XmlLoadOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstellen Sie neue XML-Ladeoptionen
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Festlegen, um numerische oder Datumswerte zu konvertieren
            options.ConvertNumericOrDate = true;
            
            // Arbeitsmappe mit Optionen laden
            Workbook workbook = new Workbook("input.xml", options);
            
            // Zugriff auf Zellen­daten
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell Value: " + cell.Value);
            Console.WriteLine("Cell Type: " + cell.Type);
            
            // Arbeitsmappe speichern.
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Stellt die Optionen zum Laden einer XML‑Datei dar.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | LoadFormat | Der Ladeformattyp. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellen Sie eine XmlLoadOptions-Instanz mit dem LoadFormat-Parameter
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // Legen Sie einige Eigenschaften von XmlLoadOptions fest
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // Eine Arbeitsmappe mit den Ladeoptionen erstellen
                Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);

                // Greife auf das erste Arbeitsblatt zu
                Worksheet worksheet = workbook.Worksheets[0];

                // Zeigen Sie einige Informationen an
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // Speichere die Arbeitsmappe
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


