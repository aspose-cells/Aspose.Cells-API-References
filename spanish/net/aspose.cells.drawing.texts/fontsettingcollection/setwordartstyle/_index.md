---
title: "FontSettingCollection.SetWordArtStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontSettingCollection. Establece el estilo WordArt predefinido"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/setwordartstyle/
---
## FontSettingCollection.SetWordArtStyle method

Establece el estilo predefinido de WordArt.

```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | PresetWordArtStyle | El estilo WordArt predefinido. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodSetWordArtStyleDemo
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
            fontSettingCollection.Text = "Sample Text for WordArt Styling";

            try
            {
                // Llama al método SetWordArtStyle con WordArtStyle7 (Relleno degradado - Azul, Acento 1, Reflexión)
                fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);

                Console.WriteLine("WordArt style applied successfully to the text box.");

                // Guardar el libro de trabajo para mostrar el efecto
                workbook.Save("FontSettingCollectionSetWordArtStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


