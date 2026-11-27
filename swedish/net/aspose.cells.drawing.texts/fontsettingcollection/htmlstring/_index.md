---
title: "FontSettingCollection.HtmlString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection-egenskap. Hämtar och anger HTML-strängen som innehåller data och vissa format i detta format"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/htmlstring/
---
## FontSettingCollection.HtmlString property

Hämtar och anger HTML‑strängen som innehåller data och vissa format i denna form.

```csharp
public string HtmlString { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 300, 100);
            var fontSettingCollection = textBox.TextBody;

            // Ange initial text med HTML-formatering
            string initialHtml = "<b>Bold Text</b> and <i>Italic Text</i>";
            fontSettingCollection.HtmlString = initialHtml;

            // Visa den aktuella HTML-strängen
            Console.WriteLine("Initial HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text: " + fontSettingCollection.Text);

            // Modifiera HTML-strängen för att lägga till mer formatering
            string modifiedHtml = "<font color='red'>Red Text</font> and <u>Underlined Text</u>";
            fontSettingCollection.HtmlString = modifiedHtml;

            // Visa de modifierade värdena
            Console.WriteLine("\nModified HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text after modification: " + fontSettingCollection.Text);

            // Lägg till en cell med HTML-formaterad text
            var cell = worksheet.Cells["A1"];
            cell.HtmlString = "<b>Cell HTML</b> <i>Formatted</i> <font color='blue'>Text</font>";

            // Spara arbetsboken för att visa både textruta och cellens HTML-formatering
            workbook.Save("FontSettingCollectionHtmlStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


