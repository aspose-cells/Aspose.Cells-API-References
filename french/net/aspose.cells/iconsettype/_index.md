---
title: "Énumération IconSetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.IconSetType. Type d’ensemble d’icônes pour le formatage conditionnel. Les valeurs seuil pour déclencher les différentes icônes au sein d’un ensemble sont configurables et l’ordre des icônes est réversible"
type: docs
url: /fr/net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Type d'ensemble d'icônes pour le formatage conditionnel. Les valeurs seuil pour déclencher les différentes icônes d'un ensemble sont configurables, et l'ordre des icônes est réversible.

```csharp
public enum IconSetType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Arrows3 | `0` | Ensemble d’icônes 3 flèches. |
| ArrowsGray3 | `1` | Ensemble d’icônes 3 flèches grises. |
| Flags3 | `2` | Ensemble d’icônes 3 drapeaux. |
| Signs3 | `3` | Ensemble d’icônes 3 signes. |
| Symbols3 | `4` | Ensemble d’icônes 3 symboles (cerclés). |
| Symbols32 | `5` | Ensemble d’icônes 3 symboles (non cerclés). |
| TrafficLights31 | `6` | Ensemble d’icônes 3 feux tricolores (sans bordure). |
| TrafficLights32 | `7` | Ensemble d’icônes 3 feux tricolores avec bordure noire épaisse. |
| Arrows4 | `8` | Ensemble d’icônes 4 flèches. |
| ArrowsGray4 | `9` | Ensemble d’icônes 4 flèches grises. |
| Rating4 | `10` | Ensemble d’icônes 4 évaluations. |
| RedToBlack4 | `11` | Ensemble d’icônes 4 'rouge à noir'. |
| TrafficLights4 | `12` | Ensemble d’icônes 4 feux tricolores. |
| Arrows5 | `13` | Jeu d'icônes de 5 flèches. |
| ArrowsGray5 | `14` | Jeu d'icônes de 5 flèches grises. |
| Quarters5 | `15` | Jeu d'icônes de 5 quarts. |
| Rating5 | `16` | Jeu d'icônes de notation 5. |
| Stars3 | `17` | Jeu de 3 étoiles |
| Boxes5 | `18` | Jeu de 5 boîtes |
| Triangles3 | `19` | Jeu de 3 triangles |
| None | `20` | Aucun |
| CustomSet | `21` | CustomSet. Cet élément est en lecture seule. |
| Smilies3 | `22` | 3 émoticônes. Seulement pour .ods. |
| ColorSmilies3 | `23` | 3 émoticônes colorées. Seulement pour .ods. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIconSetTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Définir des valeurs d'exemple
            cells["A1"].PutValue(1);
            cells["A2"].PutValue("#DIV/0!");
            cells["A3"].PutValue(3);

            // Ajouter une mise en forme conditionnelle avec un jeu d'icônes
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            fc.IconSet.Type = IconSetType.TrafficLights31;

            // Obtenir et afficher les résultats
            ConditionalFormattingResult res1 = cells["A1"].GetConditionalFormattingResult();
            Console.WriteLine($"A1 Icon Type: {res1.ConditionalFormattingIcon.Type}, Index: {res1.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res3 = cells["A3"].GetConditionalFormattingResult();
            Console.WriteLine($"A3 Icon Type: {res3.ConditionalFormattingIcon.Type}, Index: {res3.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res2 = cells["A2"].GetConditionalFormattingResult();
            Console.WriteLine($"A2 has formatting: {res2 != null && res2.ConditionalFormattingIcon != null}");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


