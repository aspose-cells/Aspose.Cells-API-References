---
title: "TextOptions.LanguageCode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Obtiene y establece el idioma de la interfaz de usuario"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

Obtiene y establece el idioma de la interfaz de usuario.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma y establecer su texto
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // Establecer el código de idioma para las opciones de texto de la forma
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // Verificar y mostrar el código de idioma
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // Guarda el libro de trabajo
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


