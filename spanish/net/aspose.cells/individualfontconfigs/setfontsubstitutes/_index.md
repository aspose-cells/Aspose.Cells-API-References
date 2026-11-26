---
title: "IndividualFontConfigs.SetFontSubstitutes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IndividualFontConfigs. Establece nombres de sustitutos de fuentes para un nombre de fuente original dado"
type: docs
url: /es/net/aspose.cells/individualfontconfigs/setfontsubstitutes/
---
## IndividualFontConfigs.SetFontSubstitutes method

Establece los nombres de fuentes sustitutas para un nombre de fuente original dado.

```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| originalFontName | String | Nombre de fuente original. |
| substituteFontNames | String[] | Lista de nombres de fuentes sustitutas que se usarán si la fuente original no está presente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Crear una instancia de IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Nombre de fuente original y sus sustitutos
            string originalFont = "Arial";
            string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };

            try
            {
                // Llamar a SetFontSubstitutes con los parámetros especificados
                fontConfigs.SetFontSubstitutes(originalFont, substitutes);

                Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
                Console.WriteLine("Substitutes are:");
                foreach (var sub in substitutes)
                {
                    Console.WriteLine($"- {sub}");
                }

                // Crear un libro de trabajo para demostrar el efecto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Establecer estilo con la fuente original
                Style style = workbook.CreateStyle();
                style.Font.Name = originalFont;
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].Value = "This text uses " + originalFont;
                worksheet.Cells["A1"].SetStyle(style);

                // Guarda el libro de trabajo
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font substitutes: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


