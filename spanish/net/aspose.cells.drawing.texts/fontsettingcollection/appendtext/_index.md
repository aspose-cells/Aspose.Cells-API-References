---
title: "FontSettingCollection.AppendText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontSettingCollection. Añade el texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/appendtext/
---
## FontSettingCollection.AppendText method

Añade el texto.

```csharp
public void AppendText(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodAppendTextWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Establece el texto inicial
            fontSettingCollection.Text = "Hello, ";

            try
            {
                // Llama al método AppendText para añadir texto adicional
                fontSettingCollection.AppendText("World!");

                // Muestra el texto modificado
                Console.WriteLine("Text after append: " + fontSettingCollection.Text);

                // Guarda el libro de trabajo
                workbook.Save("FontSettingCollectionAppendTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AppendText method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


