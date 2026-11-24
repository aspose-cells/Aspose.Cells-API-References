---
title: "FontConfigs.PreferSystemFontSubstitutes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs‑Eigenschaft. Gibt an, ob System‑Schriftart‑Ersetzungen zuerst verwendet werden sollen, wenn eine Schriftart nicht vorhanden ist und die Ersetzung dieser Schriftart nicht festgelegt ist. z. B. unter Ubuntu wird die Schriftart Arial in der Regel durch Liberation Sans ersetzt. Standardwert ist false"
type: docs
url: /de/net/aspose.cells/fontconfigs/prefersystemfontsubstitutes/
---
## FontConfigs.PreferSystemFontSubstitutes property

Gibt an, ob System-Schriftart-Ersatz zuerst verwendet werden soll, wenn eine Schriftart nicht vorhanden ist und kein Ersatz für diese Schriftart festgelegt ist. z. B. unter Ubuntu wird die Schriftart "Arial" normalerweise durch "Liberation Sans" ersetzt. Standardwert ist false.

```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktuellen Wert von PreferSystemFontSubstitutes anzeigen
            Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);

            // Setzen Sie PreferSystemFontSubstitutes auf true
            FontConfigs.PreferSystemFontSubstitutes = true;
            Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);

            // Erstellen Sie eine Zelle mit einer Schriftart, die möglicherweise ersetzt werden muss
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with Arial font");
            Style style = cell.GetStyle();
            style.Font.Name = "Arial";
            cell.SetStyle(style);

            // Speichern Sie die Arbeitsmappe, um die Auswirkungen von Schriftart‑Ersetzungen zu sehen
            workbook.Save("FontSubstitutionDemo.xlsx");

            // Auf den Standardwert zurücksetzen
            FontConfigs.PreferSystemFontSubstitutes = false;
            Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
        }
    }
}
```

### Siehe auch

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


