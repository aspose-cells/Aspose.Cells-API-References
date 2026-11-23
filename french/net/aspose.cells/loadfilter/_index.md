---
title: "Classe LoadFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LoadFilter. Représente le filtre qui fournit des options pour le chargement des données lors du chargement d'un classeur à partir d'un modèle"
type: docs
url: /fr/net/aspose.cells/loadfilter/
---
## LoadFilter class

Représente le filtre qui fournit des options de chargement des données lors du chargement d'un classeur à partir d'un modèle.

```csharp
public class LoadFilter
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | Construit un LoadFilter avec les options de filtre par défaut LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | Construit un LoadFilter avec les options de filtre fournies. |

## Propriétés

| Nom | Description |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | Les options de filtre pour indiquer quelles données doivent être chargées. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | Spécifie les feuilles (indices) et l'ordre à charger. La valeur par défaut est null, ce qui indique de charger toutes les feuilles dans l'ordre par défaut du fichier modèle. Si la valeur n'est pas null et que l'indice d'une feuille n'est pas présent dans le tableau retourné, alors la feuille ne sera pas chargée. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | Prépare les options de filtre avant de charger la feuille de calcul donnée. L'implémentation de LoadFilter par l'utilisateur peut modifier les LoadDataFilterOptions ici pour indiquer comment charger les données pour cette feuille de calcul. |

### Remarques

L'utilisateur peut spécifier les options de filtre ou implémenter son propre LoadFilter pour indiquer comment charger les données.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterDemo
    {
        public static void LoadFilterExample()
        {
            // Créez LoadOptions et définissez LoadFilter
            LoadOptions opts = new LoadOptions();
            opts.LoadFilter = new CustomLoadFilter();

            // Chargez le classeur avec les LoadOptions spécifiés
            Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);

            // Enregistrez le classeur pour voir l'effet du LoadFilter
            wb.Save("LoadFilterExample.xlsx");
        }

        // Implémentation personnalisée de LoadFilter
        public class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


