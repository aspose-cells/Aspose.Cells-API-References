---
title: "FontSettingCollection.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSettingCollection. Obtiene y establece el texto de la forma"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/text/
---
## FontSettingCollection.Text property

Obtiene y establece el texto de la forma.

```csharp
public string Text { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionPropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            try
            {
                // Establece el texto inicial
                fontSettingCollection.Text = "Initial Text Value";
                Console.WriteLine("Initial Text value: " + fontSettingCollection.Text);

                // Modifique el texto
                fontSettingCollection.Text = "Modified Text Value";
                Console.WriteLine("Modified Text value: " + fontSettingCollection.Text);

                // Demuestra la adición de texto
                fontSettingCollection.AppendText(" (Appended)");
                Console.WriteLine("After AppendText: " + fontSettingCollection.Text);

                // Guarda el libro de trabajo
                workbook.Save("FontSettingCollectionTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


