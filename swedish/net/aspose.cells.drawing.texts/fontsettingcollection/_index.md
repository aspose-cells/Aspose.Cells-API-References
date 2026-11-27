---
title: "Klass FontSettingCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.FontSettingCollection‑klass. Representerar listan av FontSetting"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/
---
## FontSettingCollection class

Representerar listan av [`FontSetting`](../../aspose.cells/fontsetting/).

```csharp
public class FontSettingCollection : CollectionBase<FontSetting>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [HtmlString](../../aspose.cells.drawing.texts/fontsettingcollection/htmlstring/) { get; set; } | Hämtar och anger HTML‑strängen som innehåller data och vissa format i denna form. |
| [Item](../../aspose.cells.drawing.texts/fontsettingcollection/item/) { get; } | Hämtar [`FontSetting`](../../aspose.cells/fontsetting/) efter indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Text](../../aspose.cells.drawing.texts/fontsettingcollection/text/) { get; set; } | Hämtar och anger texten för formen. |
| [TextAlignment](../../aspose.cells.drawing.texts/fontsettingcollection/textalignment/) { get; } | Representerar justeringsinställningen för textkroppen. |
| [TextParagraphs](../../aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/) { get; } | Hämtar alla stycken. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AppendText](../../aspose.cells.drawing.texts/fontsettingcollection/appendtext/)(string) | Lägger till texten. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [Clear](../../aspose.cells.drawing.texts/fontsettingcollection/clear/#clear)() | Rensa alla inställningar. (2 metoder) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FontSetting) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FontSetting[], int, int) |  |
| [DeleteText](../../aspose.cells.drawing.texts/fontsettingcollection/deletetext/)(int, int) | Ta bort vissa tecken. |
| override [Equals](../../aspose.cells.drawing.texts/fontsettingcollection/equals/)(object) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FontSetting&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FontSetting&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FontSetting&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FontSetting&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FontSetting&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FontSetting&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FontSetting&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FontSetting&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FontSetting&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FontSetting&gt;) |  |
| [Format](../../aspose.cells.drawing.texts/fontsettingcollection/format/)(int, int, Font, StyleFlag) | Formatera texten med font‑inställning. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| override [GetHashCode](../../aspose.cells.drawing.texts/fontsettingcollection/gethashcode/)() |  |
| [GetParagraphEnumerator](../../aspose.cells.drawing.texts/fontsettingcollection/getparagraphenumerator/)() | Hämtar enumeratorn för styckena. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int, int) |  |
| [InsertText](../../aspose.cells.drawing.texts/fontsettingcollection/inserttext/)(int, string) | Infoga indexet på positionen. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace_1)(string, string) | Ersätt texten. |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace)(int, int, string) | Ersätt texten. |
| [SetWordArtStyle](../../aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/)(PresetWordArtStyle) | Ställer in den förinställda WordArt-stilen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassFontSettingCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettings = textBox.TextBody;

            // Ange ursprunglig text
            fontSettings.Text = "Initial Text";
            Console.WriteLine("Initial Text: " + fontSettings.Text);

            // Lägg till text
            fontSettings.AppendText("\nAppended Text");
            Console.WriteLine("After Append: " + fontSettings.Text);

            // Infoga text
            fontSettings.InsertText(7, "Inserted ");
            Console.WriteLine("After Insert: " + fontSettings.Text);

            // Ersätt text efter position
            fontSettings.Replace(0, 7, "Modified");
            Console.WriteLine("After Position Replace: " + fontSettings.Text);

            // Ersätt text efter värde
            fontSettings.Replace("Appended", "Replaced");
            Console.WriteLine("After Value Replace: " + fontSettings.Text);

            // Formatera text
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.Color = System.Drawing.Color.Red;

            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontColor = true;

            fontSettings.Format(0, 8, style.Font, flag);

            // Demonstrera HTML-sträng
            fontSettings.HtmlString = "<b>Bold HTML</b> <i>Italic HTML</i>";
            Console.WriteLine("HTML String: " + fontSettings.HtmlString);

            // Kom åt textstycken
            var paragraphs = fontSettings.TextParagraphs;
            Console.WriteLine("Paragraph Count: " + paragraphs.Count);

            // Ange WordArt-stil
            fontSettings.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);

            // Spara arbetsboken
            workbook.Save("TextsClassFontSettingCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


