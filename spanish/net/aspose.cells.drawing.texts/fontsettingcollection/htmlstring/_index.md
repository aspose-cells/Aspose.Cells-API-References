---
title: "FontSettingCollection.HtmlString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSettingCollection. Obtiene y establece la cadena html que contiene datos y algunos formatos en esta forma"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/htmlstring/
---
## FontSettingCollection.HtmlString property

Obtiene y establece la cadena html que contiene datos y algunos formatos en esta forma.

```csharp
public string HtmlString { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 300, 100);
            var fontSettingCollection = textBox.TextBody;

            // Establece el texto inicial con formato HTML
            string initialHtml = "<b>Bold Text</b> and <i>Italic Text</i>";
            fontSettingCollection.HtmlString = initialHtml;

            // Muestra la cadena HTML actual
            Console.WriteLine("Initial HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text: " + fontSettingCollection.Text);

            // Modifica la cadena HTML para añadir más formato
            string modifiedHtml = "<font color='red'>Red Text</font> and <u>Underlined Text</u>";
            fontSettingCollection.HtmlString = modifiedHtml;

            // Muestra los valores modificados
            Console.WriteLine("\nModified HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text after modification: " + fontSettingCollection.Text);

            // Añade una celda con texto formateado en HTML
            var cell = worksheet.Cells["A1"];
            cell.HtmlString = "<b>Cell HTML</b> <i>Formatted</i> <font color='blue'>Text</font>";

            // Guarda el libro de trabajo para mostrar tanto el cuadro de texto como el formato HTML de la celda
            workbook.Save("FontSettingCollectionHtmlStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


