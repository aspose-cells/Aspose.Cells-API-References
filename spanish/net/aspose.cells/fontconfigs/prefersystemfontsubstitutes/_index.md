---
title: "FontConfigs.PreferSystemFontSubstitutes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontConfigs. Indica si se deben usar sustitutos de fuentes del sistema primero o no cuando una fuente no está presente y el sustituto de esa fuente no está configurado. p. ej. En Ubuntu la fuente Arial generalmente se sustituye por Liberation Sans. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/fontconfigs/prefersystemfontsubstitutes/
---
## FontConfigs.PreferSystemFontSubstitutes property

Indique si se deben usar sustitutos de fuentes del sistema primero o no cuando una fuente no está presente y el sustituto de esa fuente no está configurado. Por ejemplo, en Ubuntu, la fuente "Arial" suele ser sustituida por "Liberation Sans". El valor predeterminado es false.

```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Mostrar el valor actual de PreferSystemFontSubstitutes
            Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);

            // Establecer PreferSystemFontSubstitutes a true
            FontConfigs.PreferSystemFontSubstitutes = true;
            Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);

            // Crear una celda con una fuente que podría necesitar sustitución
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with Arial font");
            Style style = cell.GetStyle();
            style.Font.Name = "Arial";
            cell.SetStyle(style);

            // Guardar el libro de trabajo para ver los efectos de sustitución de fuentes
            workbook.Save("FontSubstitutionDemo.xlsx");

            // Restablecer al valor predeterminado
            FontConfigs.PreferSystemFontSubstitutes = false;
            Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
        }
    }
}
```

### Ver también

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


