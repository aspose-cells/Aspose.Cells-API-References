---
title: "IndividualFontConfigs.GetFontSubstitutes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IndividualFontConfigs. Devuelve una matriz que contiene nombres de sustitutos de fuentes que se usarán si la fuente original no está presente"
type: docs
url: /es/net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

Devuelve una matriz que contiene nombres de fuentes sustitutas que se usarán si la fuente original no está presente.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Valor de retorno

Una matriz que contiene nombres de sustitutos de fuentes que se usarán si la fuente original no está presente.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Crear configuraciones de fuentes individuales
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Establecer sustitutos de fuentes para "Arial"
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // Obtener sustitutos de fuentes para "Arial"
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // Crear un libro de trabajo para demostrar el efecto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Establecer estilo con la fuente original
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // Guarda el libro de trabajo
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


