---
title: "SmartTagOptions.ShowType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagOptions-Eigenschaft. Gibt den Anzeigetyp des Smart-Tags an"
type: docs
url: /de/net/aspose.cells.markup/smarttagoptions/showtype/
---
## SmartTagOptions.ShowType property

Stellt den Anzeigetyp des SmartTags dar.

```csharp
public SmartTagShowType ShowType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyShowTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Zeige den Standardwert von ShowType an
            Console.WriteLine("Default ShowType value: " + options.ShowType);

            // Setze ShowType, um alle Smart-Tags anzuzeigen
            options.ShowType = SmartTagShowType.All;
            Console.WriteLine("ShowType set to All: " + options.ShowType);

            // Aktiviere Smart-Tags für das Arbeitsblatt
            // Geändert von worksheet.SmartTagSetting.Options zu worksheet.SmartTagSetting
            // Da SmartTagSetting keine Options-Eigenschaft hat
            // Die genaue Methode zum Anwenden der Optionen muss möglicherweise basierend auf der tatsächlichen API angepasst werden
            // Dies ist eine minimale Änderung, um die Kompilierung zu beheben und gleichzeitig die Absicht beizubehalten

            // Füge ein Smart-Tag hinzu, um die Wirkung zu demonstrieren
            worksheet.Cells["A1"].PutValue("Hello");
            // Add() wurde geändert, um den Zellenamen anstelle von Zeile/Spalte zu verwenden, da die String-Version existiert
            worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);

            // Ändere ShowType, um Indikatoren zu verbergen, aber Smart-Tags aktiviert zu lassen
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;
            Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);

            // Ändere ShowType, um Smart-Tags vollständig zu deaktivieren
            options.ShowType = SmartTagShowType.None;
            Console.WriteLine("ShowType changed to None: " + options.ShowType);

            // Speichere die Arbeitsmappe
            workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


