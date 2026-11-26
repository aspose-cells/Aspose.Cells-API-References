---
title: "FontSettingCollection.Format"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontSettingCollection. Formatea el texto con la configuración de fuente"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/format/
---
## FontSettingCollection.Format method

Formatea el texto con la configuración de fuente.

```csharp
public void Format(int startIndex, int length, Font font, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice de inicio. |
| longitud | Int32 | La longitud. |
| fuente | Fuente | La fuente. |
| bandera | StyleFlag | Las banderas de la fuente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodFormatWithInt32Int32FontStyleFlagDemo
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
            fontSettingCollection.Text = "Sample Text for Formatting";

            try
            {
                // Crea un estilo y establece sus propiedades de fuente
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                style.Font.IsBold = true;
                style.Font.Color = System.Drawing.Color.Red;

                // Crear una bandera de estilo para especificar qué propiedades de fuente aplicar
                StyleFlag styleFlag = new StyleFlag();
                styleFlag.FontName = true;
                styleFlag.FontSize = true;
                styleFlag.FontBold = true;
                styleFlag.FontColor = true;

                // Formatea los caracteres del índice 7 al 11 (la palabra "Text")
                fontSettingCollection.Format(7, 4, style.Font, styleFlag);

                // Guardar el libro de trabajo para mostrar el efecto
                workbook.Save("FontSettingCollectionFormatDemo.xlsx");
                Console.WriteLine("Format method executed successfully. Text 'Text' is now bold, red Arial 14pt.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


