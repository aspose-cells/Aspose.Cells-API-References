---
title: "Enum LoadDataFilterOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.LoadDataFilterOptions. Représente les options de filtrage des données lors du chargement d’un classeur à partir d’un modèle"
type: docs
url: /fr/net/aspose.cells/loaddatafilteroptions/
---
## LoadDataFilterOptions enumeration

Représente les options de filtrage des données lors du chargement du classeur à partir d'un modèle.

```csharp
public enum LoadDataFilterOptions
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Load nothing for sheet data |
| All | `2147483647` | Tout charger |
| CellBlank | `1` | Charger les cellules dont la valeur est vide |
| CellString | `2` | Charger les cellules dont la valeur est une chaîne |
| CellNumeric | `4` | Charger les cellules dont la valeur est numérique (y compris la date/heure) |
| CellError | `8` | Charger les cellules dont la valeur est une erreur |
| CellBool | `16` | Charger les cellules dont la valeur est bool |
| CellValue | `31` | Charger uniquement la valeur des cellules (tous les types de valeur) |
| Formula | `32` | Charger les formules des cellules. |
| CellData | `67108927` | Charger les données des cellules, y compris les valeurs, les formules et le formatage |
| Chart | `256` | Charger les graphiques |
| Shape | `402653696` | Charger les formes |
| Drawing | `402653952` | Objets de dessin (incluant Chart, Picture, OleObject et tous les autres objets de dessin) |
| MergedArea | `1024` | Charger les cellules fusionnées |
| ConditionalFormatting | `2048` | Charger le formatage conditionnel |
| DataValidation | `4096` | Charger les validations de données |
| PivotTable | `8192` | Charger les tableaux croisés dynamiques |
| Table | `16384` | Charger les tableaux |
| Hyperlinks | `32768` | Charger les hyperliens |
| SheetSettings | `65536` | Charger les paramètres de la feuille de calcul |
| SheetData | `403701759` | Charger toutes les données de la feuille de calcul, telles que les données des cellules, les paramètres, les objets, ...etc. |
| BookSettings | `1048576` | Charger les paramètres du classeur |
| Settings | `1114112` | Charger les paramètres du classeur et de la feuille de calcul |
| XmlMap | `2097152` | Charger XmlMap |
| Structure | `4194304` | Charger la structure du classeur |
| DocumentProperties | `8388608` | Charger les propriétés du document |
| DefinedNames | `16777216` | Charger les objets Name définis |
| VBA | `33554432` | Charger les projets VBA |
| Style | `67108864` | Charger les styles de formatage des cellules |
| Picture | `134217728` | Charger les images |
| OleObject | `268435456` | Charger les OleObjects |
| Revision | `536870912` | Charger les journaux de révision |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadDataFilterOptionsDemo
    {
        public static void LoadDataFilterOptionsExample()
        {
            // Créer une nouvelle instance de LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Créer une implémentation personnalisée de LoadFilter
            loadOptions.LoadFilter = new CustomLoadFilter();

            // Chargez le classeur avec les options de chargement spécifiées
            Workbook workbook = new Workbook("LoadDataFilterOptionsExample_original.xlsx", loadOptions);

            // Enregistrer le classeur pour vérifier les données chargées
            workbook.Save("LoadDataFilterOptionsExample.xlsx");
        }

        // Implémentation personnalisée de LoadFilter
        private class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                // Appliquer différentes options de filtre en fonction du nom de la feuille
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


