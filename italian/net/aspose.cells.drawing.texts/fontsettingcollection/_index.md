---
title: "Classe FontSettingCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Texts.FontSettingCollection. Rappresenta l'elenco di FontSetting"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/
---
## FontSettingCollection class

Rappresenta l'elenco di [`FontSetting`](../../aspose.cells/fontsetting/).

```csharp
public class FontSettingCollection : CollectionBase<FontSetting>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [HtmlString](../../aspose.cells.drawing.texts/fontsettingcollection/htmlstring/) { get; set; } | Ottiene e imposta la stringa html che contiene dati e alcuni formati in questa forma. |
| [Item](../../aspose.cells.drawing.texts/fontsettingcollection/item/) { get; } | Ottiene il [`FontSetting`](../../aspose.cells/fontsetting/) per indice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Text](../../aspose.cells.drawing.texts/fontsettingcollection/text/) { get; set; } | Ottiene e imposta il testo della forma. |
| [TextAlignment](../../aspose.cells.drawing.texts/fontsettingcollection/textalignment/) { get; } | Rappresenta l'impostazione di allineamento del corpo del testo. |
| [TextParagraphs](../../aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/) { get; } | Ottiene tutti i paragrafi. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AppendText](../../aspose.cells.drawing.texts/fontsettingcollection/appendtext/)(string) | Aggiunge il testo. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [Clear](../../aspose.cells.drawing.texts/fontsettingcollection/clear/#clear)() | Cancella tutte le impostazioni. (2 metodi) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FontSetting) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FontSetting[], int, int) |  |
| [DeleteText](../../aspose.cells.drawing.texts/fontsettingcollection/deletetext/)(int, int) | Elimina alcuni caratteri. |
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
| [Format](../../aspose.cells.drawing.texts/fontsettingcollection/format/)(int, int, Font, StyleFlag) | Formatta il testo con l'impostazione del font. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| override [GetHashCode](../../aspose.cells.drawing.texts/fontsettingcollection/gethashcode/)() |  |
| [GetParagraphEnumerator](../../aspose.cells.drawing.texts/fontsettingcollection/getparagraphenumerator/)() | Ottiene l'enumeratore dei paragrafi. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int, int) |  |
| [InsertText](../../aspose.cells.drawing.texts/fontsettingcollection/inserttext/)(int, string) | Inserisce l'indice nella posizione. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace_1)(string, string) | Sostituisce il testo. |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace)(int, int, string) | Sostituisce il testo. |
| [SetWordArtStyle](../../aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/)(PresetWordArtStyle) | Imposta lo stile predefinito di WordArt. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettings = textBox.TextBody;

            // Imposta il testo iniziale
            fontSettings.Text = "Initial Text";
            Console.WriteLine("Initial Text: " + fontSettings.Text);

            // Aggiungi testo
            fontSettings.AppendText("\nAppended Text");
            Console.WriteLine("After Append: " + fontSettings.Text);

            // Inserisci testo
            fontSettings.InsertText(7, "Inserted ");
            Console.WriteLine("After Insert: " + fontSettings.Text);

            // Sostituisci il testo per posizione
            fontSettings.Replace(0, 7, "Modified");
            Console.WriteLine("After Position Replace: " + fontSettings.Text);

            // Sostituisci il testo per valore
            fontSettings.Replace("Appended", "Replaced");
            Console.WriteLine("After Value Replace: " + fontSettings.Text);

            // Formatta testo
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.Color = System.Drawing.Color.Red;

            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontColor = true;

            fontSettings.Format(0, 8, style.Font, flag);

            // Dimostra la stringa HTML
            fontSettings.HtmlString = "<b>Bold HTML</b> <i>Italic HTML</i>";
            Console.WriteLine("HTML String: " + fontSettings.HtmlString);

            // Accedi ai paragrafi di testo
            var paragraphs = fontSettings.TextParagraphs;
            Console.WriteLine("Paragraph Count: " + paragraphs.Count);

            // Imposta lo stile WordArt
            fontSettings.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);

            // Salva la cartella di lavoro
            workbook.Save("TextsClassFontSettingCollectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


