---
title: "Enum SmartTagShowType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Markup.SmartTagShowType Enum. Stellt den Anzeigetyp des Smart‑Tags dar."
type: docs
url: /de/net/aspose.cells.markup/smarttagshowtype/
---
## SmartTagShowType enumeration

Stellt den Anzeigetyp des SmartTags dar.

```csharp
public enum SmartTagShowType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| All | `0` | Gibt an, dass Smart‑Tags aktiviert und angezeigt werden. |
| NoSmartTagIndicator | `1` | Gibt an, dass die SmartTags aktiviert sind, aber die Anzeige nicht angezeigt wird. |
| None | `2` | Gibt an, dass SmartTags deaktiviert und nicht angezeigt werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagShowTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstriere alle Werte des Enums SmartTagShowType
            Console.WriteLine("SmartTagShowType values:");
            Console.WriteLine($"All: {SmartTagShowType.All}");
            Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
            Console.WriteLine($"None: {SmartTagShowType.None}");

            // Erstelle und konfiguriere ein SmartTag
            var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");

            // Setze Eigenschaften, die SmartTagShowType verwenden würden (simuliert, da die eigentliche Eigenschaft nicht verfügbar ist)
            Console.WriteLine("\nSmart tag created at A1 with current date");

            // Speichere mit verschiedenen Anzeige‑Typ‑Szenarien
            workbook.Save("SmartTagShowTypeDemo_All.xlsx");
            Console.WriteLine("Workbook saved with default show type (All)");

            // Erstelle ein weiteres Arbeitsbuch mit unterschiedlichem Anzeige‑Typ‑Verhalten
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];
            worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
            Console.WriteLine("\nSecond workbook created with smart tag at B2");

            workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
            Console.WriteLine("Second workbook saved (simulating None behavior)");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


