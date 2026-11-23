---
title: "Classe SmartTagOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Markup.SmartTagOptions. Représente les options du smart tag"
type: docs
url: /fr/net/aspose.cells.markup/smarttagoptions/
---
## SmartTagOptions class

Représente les options de la balise intelligente.

```csharp
public class SmartTagOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | Indique si les smart tags sont enregistrés avec le classeur. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | Représente le type d'affichage du smart tag. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Définir les propriétés
            options.EmbedSmartTags = true;
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;

            // Appliquer SmartTagOptions à la feuille de calcul
            // Remarque : Modifié de worksheet.SmartTagSetting.Options = options;
            // pour utiliser directement l'objet options car SmartTagSetting n'a pas de propriété Options
            // (En supposant que les options sont destinées à être utilisées directement)
            
            // Ajouter des données pour démontrer
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);

            // Enregistrez le classeur
            workbook.Save("SmartTagOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


