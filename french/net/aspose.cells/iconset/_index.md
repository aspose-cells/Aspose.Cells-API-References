---
title: "Classe IconSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.IconSet class. Décrivez la règle de mise en forme conditionnelle IconSet. Cette règle de mise en forme conditionnelle applique des icônes aux cellules selon leurs valeurs"
type: docs
url: /fr/net/aspose.cells/iconset/
---
## IconSet class

Décrit la règle de mise en forme conditionnelle IconSet. Cette règle de mise en forme conditionnelle applique des icônes aux cellules en fonction de leurs valeurs.

```csharp
public class IconSet
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | Obtenir le[`ConditionalFormattingIcon`](../conditionalformattingicon/) de la collection |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | Obtenir l'instance CFValueObjects. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | Indique si le jeu d'icônes est personnalisé. La valeur par défaut est false. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | Obtenir ou définir le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans cet ensemble d'icônes. La valeur par défaut est false. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | Obtenir ou définir le drapeau indiquant s'il faut afficher les valeurs des cellules auxquelles cet ensemble d'icônes est appliqué. La valeur par défaut est true. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | Obtenir ou définir le type d'ensemble d'icônes à afficher. La définition du type vérifiera automatiquement si le nombre actuel de Cfvos correspond au nouveau type. Si ce n'est pas le cas, les anciens Cfvos seront supprimés et des Cfvos par défaut seront ajoutés. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetDemo
    {
        public static void IconSetExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoute une mise en forme conditionnelle vide
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Définit la plage de mise en forme conditionnelle
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Ajoute une condition
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Obtenir l'ensemble d'icônes
            IconSet iconSet = cond.IconSet;

            // Définir le type d'icône
            iconSet.Type = IconSetType.Arrows3;

            // Définir des propriétés supplémentaires
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Définir les valeurs des cellules
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Enregistrement du fichier Excel
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


