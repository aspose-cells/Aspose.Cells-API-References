---
title: "FontConfigs.DefaultFontName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontConfigs. Obtiene o establece el nombre de fuente predeterminado"
type: docs
url: /es/net/aspose.cells/fontconfigs/defaultfontname/
---
## FontConfigs.DefaultFontName property

Obtiene o establece el nombre de fuente predeterminado.

```csharp
public static string DefaultFontName { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Mostrar el nombre de fuente predeterminado actual
            Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);

            // Establecer un nuevo nombre de fuente predeterminado
            FontConfigs.DefaultFontName = "Arial";

            // Crear un estilo sin una fuente explícita establecida para demostrar el uso de la fuente predeterminada
            Style style = workbook.CreateStyle();
            style.Font.Name = ""; // Empty to use default font

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text should use the default font");
            cell.SetStyle(style);

            // Guardar el libro de trabajo para ver el efecto
            workbook.Save("PropertyDefaultFontNameDemo.xlsx");

            // Verificar que la fuente se aplicó correctamente
            Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
        }
    }
}
```

### Ver también

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


