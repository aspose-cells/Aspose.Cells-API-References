---
title: "Style.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Copie les données d'un autre objet style"
type: docs
url: /fr/net/aspose.cells/style/copy/
---
## Style.Copy method

Copie les données d'un autre objet style

```csharp
public void Copy(Style style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | Objet Style source |

### Remarques

Cette méthode ne copie pas le nom du style. Si vous souhaitez copier le nom, veuillez appeler le code suivant après la copie du style : destStyle.Name = style.Name.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCopyWithStyleDemo
    {
        public static void Run()
        {
            // Créer le classeur source avec des données d'exemple
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Sample Text");
            Style srcStyle = srcWorkbook.CreateStyle();
            srcStyle.Font.Name = "Arial";
            srcStyle.Font.Size = 14;
            srcSheet.Cells["A1"].SetStyle(srcStyle);

            // Créer le classeur de destination
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copier le style de la source vers la destination
            Style destStyle = destWorkbook.CreateStyle();
            destStyle.Copy(srcStyle);
            
            // Appliquer le style copié
            destSheet.Cells["B2"].PutValue("Copied Style Text");
            destSheet.Cells["B2"].SetStyle(destStyle);

            // Enregistrer le résultat
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


