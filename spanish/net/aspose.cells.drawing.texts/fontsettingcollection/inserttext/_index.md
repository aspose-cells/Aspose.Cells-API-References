---
title: "FontSettingCollection.InsertText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontSettingCollection. Inserta el índice en la posición"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/inserttext/
---
## FontSettingCollection.InsertText method

Inserta el índice en la posición.

```csharp
public void InsertText(int index, string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de inicio. |
| texto | String | El texto. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var fontSettingCollection = textBox.TextBody;

            // Establece el texto inicial
            fontSettingCollection.Text = "Initial Text";

            try
            {
                // Llama al método InsertText para insertar texto en el índice 7
                fontSettingCollection.InsertText(7, " Inserted");

                // Muestra el texto modificado
                Console.WriteLine("Text after insertion: " + fontSettingCollection.Text);
                
                // Guarda el libro de trabajo
                workbook.Save("FontSettingCollectionInsertTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertText method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


