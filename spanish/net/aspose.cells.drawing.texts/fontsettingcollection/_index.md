---
title: "Clase FontSettingCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.FontSettingCollection. Representa la lista de FontSetting"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/
---
## FontSettingCollection class

Representa la lista de [`FontSetting`](../../aspose.cells/fontsetting/).

```csharp
public class FontSettingCollection : CollectionBase<FontSetting>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [HtmlString](../../aspose.cells.drawing.texts/fontsettingcollection/htmlstring/) { get; set; } | Obtiene y establece la cadena html que contiene datos y algunos formatos en esta forma. |
| [Item](../../aspose.cells.drawing.texts/fontsettingcollection/item/) { get; } | Obtiene el [`FontSetting`](../../aspose.cells/fontsetting/) por el índice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Text](../../aspose.cells.drawing.texts/fontsettingcollection/text/) { get; set; } | Obtiene y establece el texto de la forma. |
| [TextAlignment](../../aspose.cells.drawing.texts/fontsettingcollection/textalignment/) { get; } | Representa la configuración de alineación del cuerpo del texto. |
| [TextParagraphs](../../aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/) { get; } | Obtiene todos los párrafos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AppendText](../../aspose.cells.drawing.texts/fontsettingcollection/appendtext/)(string) | Añade el texto. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FontSetting, IComparer&lt;FontSetting&gt;) |  |
| [Clear](../../aspose.cells.drawing.texts/fontsettingcollection/clear/#clear)() | Borra toda la configuración. (2 métodos) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FontSetting) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FontSetting[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FontSetting[], int, int) |  |
| [DeleteText](../../aspose.cells.drawing.texts/fontsettingcollection/deletetext/)(int, int) | Elimina algunos caracteres. |
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
| [Format](../../aspose.cells.drawing.texts/fontsettingcollection/format/)(int, int, Font, StyleFlag) | Formatea el texto con la configuración de fuente. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| override [GetHashCode](../../aspose.cells.drawing.texts/fontsettingcollection/gethashcode/)() |  |
| [GetParagraphEnumerator](../../aspose.cells.drawing.texts/fontsettingcollection/getparagraphenumerator/)() | Obtiene el enumerador de los párrafos. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FontSetting, int, int) |  |
| [InsertText](../../aspose.cells.drawing.texts/fontsettingcollection/inserttext/)(int, string) | Inserta el índice en la posición. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FontSetting, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace_1)(string, string) | Reemplaza el texto. |
| [Replace](../../aspose.cells.drawing.texts/fontsettingcollection/replace/#replace)(int, int, string) | Reemplaza el texto. |
| [SetWordArtStyle](../../aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/)(PresetWordArtStyle) | Establece el estilo predefinido de WordArt. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettings = textBox.TextBody;

            // Establece el texto inicial
            fontSettings.Text = "Initial Text";
            Console.WriteLine("Initial Text: " + fontSettings.Text);

            // Añadir texto
            fontSettings.AppendText("\nAppended Text");
            Console.WriteLine("After Append: " + fontSettings.Text);

            // Insertar texto
            fontSettings.InsertText(7, "Inserted ");
            Console.WriteLine("After Insert: " + fontSettings.Text);

            // Reemplazar texto por posición
            fontSettings.Replace(0, 7, "Modified");
            Console.WriteLine("After Position Replace: " + fontSettings.Text);

            // Reemplazar texto por valor
            fontSettings.Replace("Appended", "Replaced");
            Console.WriteLine("After Value Replace: " + fontSettings.Text);

            // Formatear texto
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.Color = System.Drawing.Color.Red;

            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontColor = true;

            fontSettings.Format(0, 8, style.Font, flag);

            // Demostrar cadena HTML
            fontSettings.HtmlString = "<b>Bold HTML</b> <i>Italic HTML</i>";
            Console.WriteLine("HTML String: " + fontSettings.HtmlString);

            // Acceder a los párrafos de texto
            var paragraphs = fontSettings.TextParagraphs;
            Console.WriteLine("Paragraph Count: " + paragraphs.Count);

            // Establecer estilo WordArt
            fontSettings.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);

            // Guarda el libro de trabajo
            workbook.Save("TextsClassFontSettingCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


