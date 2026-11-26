---
title: "FontConfigs.SetFontSources"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontConfigs. Establece los orígenes de fuentes"
type: docs
url: /es/net/aspose.cells/fontconfigs/setfontsources/
---
## FontConfigs.SetFontSources method

Establece las fuentes de tipografía.

```csharp
public static void SetFontSources(FontSourceBase[] sources)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| orígenes | FontSourceBase[] | Una matriz de orígenes que contienen fuentes TrueType. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Crear un archivo de fuente temporal para demostración
            string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
            try
            {
                File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo

                // Crear orígenes de fuentes
                FontSourceBase[] fontSources = new FontSourceBase[]
                {
                    new FolderFontSource(Path.GetTempPath(), true),
                    new FileFontSource(tempFontFile)
                };

                try
                {
                    // Llamar al método SetFontSources
                    FontConfigs.SetFontSources(fontSources);

                    // Verifique que los orígenes de fuentes estén configurados
                    FontSourceBase[] currentSources = FontConfigs.GetFontSources();
                    Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");

                    // Demuestre el efecto verificando si una fuente está disponible
                    bool isAvailable = FontConfigs.IsFontAvailable("Arial");
                    Console.WriteLine($"Is Arial available: {isAvailable}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
                }
            }
            finally
            {
                // Limpiar
                if (File.Exists(tempFontFile))
                {
                    File.Delete(tempFontFile);
                }
            }
        }
    }
}
```

### Ver también

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


