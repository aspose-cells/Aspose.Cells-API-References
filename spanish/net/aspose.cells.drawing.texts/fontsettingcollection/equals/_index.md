---
title: "FontSettingCollection.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontSettingCollection."
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/equals/
---
## FontSettingCollection.Equals method

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Establece algún texto
            fontSettingCollection.Text = "Sample Text";

            try
            {
                // Crea otro FontSettingCollection para comparación
                var anotherTextBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var anotherFontSettingCollection = anotherTextBox.TextBody;
                anotherFontSettingCollection.Text = "Sample Text";

                // Llama al método Equals para comparar las dos colecciones
                bool areEqual = fontSettingCollection.Equals(anotherFontSettingCollection);

                // Mostrar el resultado
                Console.WriteLine($"Are the FontSettingCollections equal? {areEqual}");

                // Guarda el libro de trabajo
                workbook.Save("FontSettingCollectionEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Equals: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


