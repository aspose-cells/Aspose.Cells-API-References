---
title: "SmartTagCollection.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagCollection-Eigenschaft. Gibt die Spalte der Zellen‑SmartTags zurück"
type: docs
url: /de/net/aspose.cells.markup/smarttagcollection/column/
---
## SmartTagCollection.Column property

Ruft die Spalte der Zellen‑SmartTags ab.

```csharp
public int Column { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Smart-Tag zu Zelle C5 (Zeile 4, Spalte 2) hinzu
            worksheet.Cells["C5"].PutValue("SmartTag Demo");
            int index = worksheet.SmartTagSetting.Add("C5");
            
            // Rufe die SmartTagCollection für Zelle C5 ab
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Zeige die Spalte der Zelle an, die diese Smart-Tags enthält
            Console.WriteLine("SmartTags are located at column: " + smartTags.Column);

            // Füge ein weiteres Smart-Tag zu Zelle E2 (Zeile 1, Spalte 4) hinzu, um eine andere Spalte zu demonstrieren
            worksheet.Cells["E2"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("E2");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);

            // Speichere die Arbeitsmappe
            workbook.Save("SmartTagColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


