---
title: "Enum ReflectionEffectType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ReflectionEffectType enum. Représente le type d'effet de réflexion"
type: docs
url: /fr/net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

Représente le type d’effet de réflexion.

```csharp
public enum ReflectionEffectType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucun effet de réflexion. |
| Custom | `1` | Effet de réflexion personnalisé. |
| TightReflectionTouching | `2` | Réflexion serrée, en contact. |
| HalfReflectionTouching | `3` | Réflexion à moitié, en contact. |
| FullReflectionTouching | `4` | Réflexion complète, en contact. |
| TightReflection4PtOffset | `5` | Réflexion serrée, décalage de 4 pt. |
| HalfReflection4PtOffset | `6` | Réflexion à moitié, décalage de 4 pt. |
| FullReflection4PtOffset | `7` | Réflexion complète, décalage de 4 pt. |
| TightReflection8PtOffset | `8` | Réflexion serrée, décalage de 8 pt. |
| HalfReflection8PtOffset | `9` | Réflexion à moitié, décalage de 8 pt. |
| FullReflection8PtOffset | `10` | Réflexion complète, décalage de 8 pt. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme rectangulaire
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Obtenir l'effet de réflexion
            ReflectionEffect reflection = rectangle.Reflection;
            
            // Définir les propriétés de réflexion
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Enregistrez le classeur
            workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
            
            Console.WriteLine("Reflection effect demo completed successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


