---
title: "FontSettingCollection.DeleteText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontSettingCollection. Elimina algunos caracteres"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/deletetext/
---
## FontSettingCollection.DeleteText method

Elimina algunos caracteres.

```csharp
public void DeleteText(int index, int count)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de inicio. |
| contar | Int32 | El recuento de caracteres. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodDeleteTextWithInt32Int32Demo
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
            fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";

            try
            {
                // Mostrar texto original
                Console.WriteLine("Original text: " + fontSettingCollection.Text);

                // Llame al método DeleteText para eliminar 7 caracteres a partir del índice 5
                fontSettingCollection.DeleteText(5, 7);

                // Mostrar texto modificado
                Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);

                // Guarda el libro de trabajo
                workbook.Save("FontSettingCollectionDeleteTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteText method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


