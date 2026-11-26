---
title: "FontConfigs.SetFontSubstitutes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontConfigs. Nombres de sustitución de fuentes para el nombre de fuente original dado"
type: docs
url: /es/net/aspose.cells/fontconfigs/setfontsubstitutes/
---
## FontConfigs.SetFontSubstitutes method

Nombres de sustitutos de fuentes para el nombre de fuente original dado.

```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
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

    public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nombre de fuente original que podría no estar disponible
            string originalFontName = "Arial";
            
            // Nombres de fuentes sustitutas para usar cuando la original no está disponible
            string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
            
            try
            {
                // Llama al método SetFontSubstitutes para configurar sustituciones de fuentes
                FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
                
                Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
                
                // Verifica las sustituciones recuperándolas
                string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("Current substitutes for '{0}':", originalFontName);
                foreach (string font in retrievedSubstitutes)
                {
                    Console.WriteLine("- " + font);
                }
                
                // Aplica la fuente a una celda para demostrar la sustitución
                worksheet.Cells["A1"].PutValue("Text with potential font substitution");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = originalFontName;
                worksheet.Cells["A1"].SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("FontSubstitutionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


