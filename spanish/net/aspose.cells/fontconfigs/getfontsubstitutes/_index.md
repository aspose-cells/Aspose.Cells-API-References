---
title: "FontConfigs.GetFontSubstitutes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontConfigs. Devuelve una matriz que contiene nombres de sustitutos de fuentes que se usarán si la fuente original no está presente"
type: docs
url: /es/net/aspose.cells/fontconfigs/getfontsubstitutes/
---
## FontConfigs.GetFontSubstitutes method

Devuelve un arreglo que contiene nombres de sustitutos de fuentes para usar si la fuente original no está presente.

```csharp
public static string[] GetFontSubstitutes(string originalFontName)
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

    public class FontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Inicializar FontConfigs
            FontConfigs fontConfigs = new FontConfigs();

            try
            {
                // Llamar a GetFontSubstitutes con un nombre de fuente
                string originalFontName = "Arial";
                string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);

                // Muestra los resultados
                Console.WriteLine($"Substitute fonts for '{originalFontName}':");
                if (substitutes != null && substitutes.Length > 0)
                {
                    foreach (string substitute in substitutes)
                    {
                        Console.WriteLine(substitute);
                    }
                }
                else
                {
                    Console.WriteLine("No substitutes found for the specified font.");
                }

                // Demostrar la configuración de sustitutos y su obtención
                string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
                FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);

                // Obtener los sustitutos nuevamente para verificar
                substitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("\nAfter setting substitutes:");
                foreach (string substitute in substitutes)
                {
                    Console.WriteLine(substitute);
                }
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

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


