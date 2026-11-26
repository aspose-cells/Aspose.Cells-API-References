---
title: "FontSettingCollection.Replace"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontSettingCollection. Reemplaza el texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

Reemplaza el texto.

```csharp
public void Replace(int index, int count, string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de inicio. |
| contar | Int32 | El recuento de caracteres. |
| texto | String | El texto. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodReplaceWithInt32Int32StringDemo
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
            fontSettingCollection.Text = "Original text to be modified";

            try
            {
                // Llame al método Replace para reemplazar 8 caracteres a partir del índice 9 con texto nuevo
                fontSettingCollection.Replace(9, 8, "replaced");

                // Muestra el texto modificado
                Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);

                // Guarda el libro de trabajo
                workbook.Save("FontSettingCollectionReplaceDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

Reemplaza el texto.

```csharp
public void Replace(string oldValue, string newValue)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldValue | String | El texto antiguo. |
| newValue | String | El texto nuevo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma y establecer texto
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample text ３４ for replacement";
            
            // Reemplazar texto en la forma
            shape.TextBody.Replace("３４", "ABC");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


