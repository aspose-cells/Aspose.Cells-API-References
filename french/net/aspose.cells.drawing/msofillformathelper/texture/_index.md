---
title: "MsoFillFormatHelper.Texture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormatHelper. Obtient le type de remplissage de texture"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Obtient le type de remplissage de texture.

```csharp
public TextureType Texture { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une étiquette pour rendre l'exemple significatif
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // Créer une instance de MsoFillFormatHelper en utilisant la réflexion (pas de constructeur public)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Afficher la valeur actuelle de la propriété Texture (lecture seule)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // Démontrer que la propriété est en lecture seule en essayant de la définir (commenté)
                // fillHelper.Texture = TextureType.Canvas; // Cela provoquerait une erreur de compilation

                // Afficher tous les types de texture disponibles à titre de référence
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // Enregistrez le classeur pour démontrer une exécution réussie
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


