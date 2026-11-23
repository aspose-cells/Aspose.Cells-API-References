---
title: "Énumération HtmlEmbeddedFontType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Rendering.HtmlEmbeddedFontType. Représente le type de police incorporée dans le html"
type: docs
url: /fr/net/aspose.cells.rendering/htmlembeddedfonttype/
---
## HtmlEmbeddedFontType enumeration

Représente le type de police incorporée dans le HTML.

```csharp
public enum HtmlEmbeddedFontType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Ne pas incorporer la police. |
| Woff | `1` | Incorporer la police WOFF. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Démontrer l'utilisation des valeurs de l'énumération HtmlEmbeddedFontType
                HtmlEmbeddedFontType noneType = HtmlEmbeddedFontType.None;
                HtmlEmbeddedFontType woffType = HtmlEmbeddedFontType.Woff;

                // Afficher les valeurs d'énumération
                Console.WriteLine("None font type: " + noneType);
                Console.WriteLine("Woff font type: " + woffType);

                // Démontrer la comparaison
                if (noneType == HtmlEmbeddedFontType.None)
                {
                    Console.WriteLine("Font type is correctly set to None");
                }

                if (woffType == HtmlEmbeddedFontType.Woff)
                {
                    Console.WriteLine("Font type is correctly set to Woff");
                }

                // Afficher les valeurs numériques
                Console.WriteLine("Numeric value for None: " + (int)noneType);
                Console.WriteLine("Numeric value for Woff: " + (int)woffType);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlEmbeddedFontType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


