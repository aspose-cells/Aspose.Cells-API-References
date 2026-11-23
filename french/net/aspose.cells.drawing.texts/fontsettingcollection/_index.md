---
title: "Classe FontSettingCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.FontSettingCollection. Représente la liste de FontSetting"
type: docs
url: /fr/net/aspose.cells.drawing.texts/fontsettingcollection/
---
## FontSettingCollection class

Représente la liste de [`FontSetting`](../../aspose.cells/fontsetting/).

```csharp
public class FontSettingCollection : CollectionBase<FontSetting>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [HtmlString](../../aspose.cells.drawing.texts/fontsettingcollection/htmlstring/) { get; set; } | Obtient et définit la chaîne html qui contient des données et certains formats dans cette forme. |
| [Item](../../aspose.cells.drawing.texts/fontsettingcollection/item/) { get; } | Obtient le [`FontSetting`](../../aspose.cells/fontsetting/) par l'index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Text](../../aspose.cells.drawing.texts/fontsettingcollection/text/) { get; set; } | Obtient et définit le texte de la forme. |
| [TextAlignment](../../aspose.cells.drawing.texts/fontsettingcollection/textalignment/) { get; } | Représente le paramètre d'alignement du corps du texte. |
| [TextParagraphs](../../aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/) { get; } | Obtient tous les paragraphes. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AppendText](../../aspose.cells.drawing.texts/fontsettingcollection/appendtext/)(string) | Ajoute le texte. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [Clear](../../aspose.cells.drawing.texts/fontsettingcollection/clear/#clear)() | Efface tous les paramètres. (2 méthodes) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FontSetting) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FontSetting[], int, int) |  |
| [DeleteText](../../aspose.cells.drawing.texts/fontsettingcollection/deletetext/)(int, int) | Supprime certains caractères. |
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
| [Format](../../aspose.cells.drawing.texts/fontsettingcollection/format/)(int, int, Font, StyleFlag) | Formate le texte avec le paramètre de police. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| override [GetHashCode](../../aspose.cells.drawing.texts/fontsettingcollection/gethashcode/)() |  |
| [GetParagraphEnumerator](../../aspose.cells.drawing.texts/fontsettingcollection/getparagraphenumerator/)() | Obtient l'énumérateur des paragraphes. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int, int) |  |
| [InsertText](../../aspose.cells.drawing.texts/fontsettingcollection/inserttext/)(int, string) | Insère l'index à la position. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace_1)(string, string) | Remplace le texte. |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace)(int, int, string) | Remplace le texte. |
| [SetWordArtStyle](../../aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/)(PresetWordArtStyle) | Définit le style WordArt prédéfini. |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettings = textBox.TextBody;

            // Définir le texte initial
            fontSettings.Text = "Initial Text";
            Console.WriteLine("Initial Text: " + fontSettings.Text);

            // Ajouter du texte
            fontSettings.AppendText("\nAppended Text");
            Console.WriteLine("After Append: " + fontSettings.Text);

            // Insérer du texte
            fontSettings.InsertText(7, "Inserted ");
            Console.WriteLine("After Insert: " + fontSettings.Text);

            // Remplacer le texte par position
            fontSettings.Replace(0, 7, "Modified");
            Console.WriteLine("After Position Replace: " + fontSettings.Text);

            // Remplacer le texte par valeur
            fontSettings.Replace("Appended", "Replaced");
            Console.WriteLine("After Value Replace: " + fontSettings.Text);

            // Formater le texte
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.Color = System.Drawing.Color.Red;

            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontColor = true;

            fontSettings.Format(0, 8, style.Font, flag);

            // Démontrer la chaîne HTML
            fontSettings.HtmlString = "<b>Bold HTML</b> <i>Italic HTML</i>";
            Console.WriteLine("HTML String: " + fontSettings.HtmlString);

            // Accéder aux paragraphes de texte
            var paragraphs = fontSettings.TextParagraphs;
            Console.WriteLine("Paragraph Count: " + paragraphs.Count);

            // Définir le style WordArt
            fontSettings.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);

            // Enregistrez le classeur
            workbook.Save("TextsClassFontSettingCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


