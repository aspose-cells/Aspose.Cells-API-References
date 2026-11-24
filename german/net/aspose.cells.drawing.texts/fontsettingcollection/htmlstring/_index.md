---
title: "FontSettingCollection.HtmlString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection-Eigenschaft. Gibt die HTML-Zeichenfolge zurück und legt sie fest, die Daten und einige Formate in dieser Form enthält"
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/htmlstring/
---
## FontSettingCollection.HtmlString property

Liest und schreibt die HTML-Zeichenfolge, die Daten und einige Formate in dieser Form enthält.

```csharp
public string HtmlString { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 300, 100);
            var fontSettingCollection = textBox.TextBody;

            // Setze den Anfangstext mit HTML-Formatierung
            string initialHtml = "<b>Bold Text</b> and <i>Italic Text</i>";
            fontSettingCollection.HtmlString = initialHtml;

            // Zeige die aktuelle HTML-Zeichenfolge an
            Console.WriteLine("Initial HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text: " + fontSettingCollection.Text);

            // Modifiziere die HTML-Zeichenfolge, um weitere Formatierungen hinzuzufügen
            string modifiedHtml = "<font color='red'>Red Text</font> and <u>Underlined Text</u>";
            fontSettingCollection.HtmlString = modifiedHtml;

            // Zeige die modifizierten Werte an
            Console.WriteLine("\nModified HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text after modification: " + fontSettingCollection.Text);

            // Füge eine Zelle mit HTML-formatiertem Text hinzu
            var cell = worksheet.Cells["A1"];
            cell.HtmlString = "<b>Cell HTML</b> <i>Formatted</i> <font color='blue'>Text</font>";

            // Speichere die Arbeitsmappe, um sowohl die Textfeld- als auch die Zellen-HTML-Formatierung anzuzeigen
            workbook.Save("FontSettingCollectionHtmlStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


