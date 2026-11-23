---
title: "IconSet.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété IconSet. Obtenir ou définir le type de jeu d'icônes à afficher. Le fait de définir le type vérifiera automatiquement si le nombre actuel de Cfvoss est conforme au nouveau type. Si ce n'est pas le cas, les anciens Cfvos seront nettoyés et des Cfvos par défaut seront ajoutés."
type: docs
url: /fr/net/aspose.cells/iconset/type/
---
## IconSet.Type property

Obtenir ou définir le type d'ensemble d'icônes à afficher. La définition du type vérifiera automatiquement si le nombre actuel de Cfvos correspond au nouveau type. Si ce n'est pas le cas, les anciens Cfvos seront supprimés et des Cfvos par défaut seront ajoutés.

```csharp
public IconSetType Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];
            IconSet iconSet = cond.IconSet;

            // Démontrer l'utilisation de la propriété Type
            iconSet.Type = IconSetType.Arrows3;

            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            workbook.Save("IconSetExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


