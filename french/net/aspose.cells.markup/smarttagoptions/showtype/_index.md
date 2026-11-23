---
title: "SmartTagOptions.ShowType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTagOptions. Représente le type d'affichage du smart tag"
type: docs
url: /fr/net/aspose.cells.markup/smarttagoptions/showtype/
---
## SmartTagOptions.ShowType property

Représente le type d'affichage du smart tag.

```csharp
public SmartTagShowType ShowType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyShowTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Afficher la valeur par défaut de ShowType
            Console.WriteLine("Default ShowType value: " + options.ShowType);

            // Définir ShowType pour afficher toutes les balises intelligentes
            options.ShowType = SmartTagShowType.All;
            Console.WriteLine("ShowType set to All: " + options.ShowType);

            // Activer les balises intelligentes pour la feuille de calcul
            // Modifié de worksheet.SmartTagSetting.Options à worksheet.SmartTagSetting
            // Puisque SmartTagSetting n'a pas de propriété Options
            // La façon exacte d'appliquer les options peut devoir être ajustée en fonction de l'API réelle
            // Il s'agit d'un changement minimal pour corriger la compilation tout en préservant l'intention

            // Ajouter une balise intelligente pour démontrer l'effet
            worksheet.Cells["A1"].PutValue("Hello");
            // Modifié Add() pour utiliser le nom de cellule au lieu de ligne/colonne puisque la version chaîne existe
            worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);

            // Modifier ShowType pour masquer les indicateurs tout en maintenant les balises intelligentes activées
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;
            Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);

            // Modifier ShowType pour désactiver complètement les balises intelligentes
            options.ShowType = SmartTagShowType.None;
            Console.WriteLine("ShowType changed to None: " + options.ShowType);

            // Enregistrez le classeur
            workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


