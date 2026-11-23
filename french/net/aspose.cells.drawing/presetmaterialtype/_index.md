---
title: "Enum PresetMaterialType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.PresetMaterialType enum. Décrit l'apparence de la surface d'une forme"
type: docs
url: /fr/net/aspose.cells.drawing/presetmaterialtype/
---
## PresetMaterialType enumeration

Décrit l’apparence de surface d’une forme.

```csharp
public enum PresetMaterialType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Clear | `0` | Clair |
| DarkEdge | `1` | Bord sombre |
| Flat | `2` | Plat |
| LegacyMatte | `3` | Mat hérité |
| LegacyMetal | `4` | Métal hérité |
| LegacyPlastic | `5` | Plastique hérité |
| LegacyWireframe | `6` | Fil de fer hérité |
| Matte | `7` | Mat |
| Metal | `8` | Métal |
| Plastic | `9` | Plastique |
| Powder | `10` | Poudre |
| SoftEdge | `11` | Bord doux |
| SoftMetal | `12` | Métal doux |
| TranslucentPowder | `13` | Poudre translucide |
| WarmMatte | `14` | Mat chaud |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class PresetMaterialTypeDemo
    {
        public static void PresetMaterialTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Accéder à la première série du graphique
            Series series = chart.NSeries[0];

            // Accéder au format 3D de la série
            Format3D format3D = series.ShapeProperties.Format3D;

            // Définir le type de matériau de surface
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // Définir d'autres propriétés 3D
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // Enregistrez le classeur
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // Afficher les résultats
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


