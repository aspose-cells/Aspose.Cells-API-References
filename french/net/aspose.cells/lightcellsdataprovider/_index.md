---
title: "Interface LightCellsDataProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.LightCellsDataProvider. Représente le fournisseur de données pour l'enregistrement de gros fichiers de feuille de calcul en mode léger."
type: docs
url: /fr/net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

Représente le fournisseur de données pour l'enregistrement de grands fichiers de feuille de calcul en mode léger.

```csharp
public interface LightCellsDataProvider
```

## Méthodes

| Nom | Description |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Vérifie si la valeur chaîne actuelle de la cellule doit être rassemblée dans un pool global. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Obtient la prochaine cellule à enregistrer. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Obtient la prochaine ligne à enregistrer. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Commence à enregistrer les données d'une cellule. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Commence à enregistrer les données d'une ligne. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Commence à enregistrer une feuille de calcul. |

### Remarques

Lors de l'enregistrement d'un classeur avec ce mode, [`StartSheet`](./startsheet/) sera vérifié lors de l'enregistrement de chaque feuille de calcul du classeur. Pour une feuille, si [`StartSheet`](./startsheet/) renvoie vrai, alors toutes les données et propriétés à enregistrer pour les lignes/cellules de cette feuille seront fournies par l'implémentation de cette interface. Tout d'abord, [`NextRow`](./nextrow/) sera appelé pour obtenir l'index de la prochaine ligne à enregistrer. Si un index de ligne valide est retourné (l'index de ligne doit être en ordre croissant pour les lignes à enregistrer), alors un objet Row représentant cette ligne sera fourni par [`StartRow`](./startrow/) pour que l'implémentation définisse ses propriétés. Pour une ligne, [`NextCell`](./nextcell/) sera vérifié en premier. Si un index de colonne valide est retourné (l'index de colonne doit être en ordre croissant pour toutes les cellules de la ligne actuelle), alors un objet Cell représentant cette cellule sera fourni par [`StartCell`](./startcell/) pour que l'implémentation définisse ses données et propriétés. Après [`StartCell`](./startcell/) la cellule sera enregistrée directement dans le fichier de feuille de calcul résultant. Ensuite, la cellule suivante sera vérifiée et traitée. Veuillez noter que l'utilisateur ne doit mettre à jour que les valeurs et propriétés de l'objet Row/Cell actuel fourni par la méthode correspondante. Parce que les données des cellules sont écrites dans le fichier résultant de manière flux, la plupart des autres objets peuvent déjà avoir été écrits dans le fichier résultant, ou avoir été rassemblés et écrit certaines données globales pour eux. Ainsi, lorsqu'un utilisateur met à jour d'autres objets pendant l'enregistrement des données des cellules, ces opérations peuvent ne pas pouvoir affecter les données enregistrées. Ou pire encore, ces opérations peuvent entraîner des données incohérentes enregistrées dans le fichier résultant et finalement corrompre le fichier. Donc, pour tous les autres objets tels que les formes, la largeur des colonnes et les styles, les mises en forme conditionnelles, ...etc., veuillez ne pas les manipuler dans aucune méthode de cette implémentation. Au lieu de cela, veuillez les gérer et les ajuster à l'état final avant d'appeler la méthode "Save" du Workbook.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderDemo
    {
        public static void LightCellsDataProviderExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un LightCellsDataProvider personnalisé
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // Définir le LightCellsDataProvider pour enregistrer le classeur
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Enregistrer le classeur avec le LightCellsDataProvider personnalisé
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Commencer le traitement de la première feuille
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            // Passer à la ligne suivante
            currentRow++;
            currentCell = -1;

            // Retourner l'index de la ligne actuelle ou -1 s'il n'y a plus de lignes
            return currentRow < 10 ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Initialiser la ligne si nécessaire
        }

        public int NextCell()
        {
            // Passer à la cellule suivante
            currentCell++;

            // Retourner l'index de la cellule actuelle ou -1 s'il n'y a plus de cellules
            return currentCell < 10 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            // Définissez la valeur de la cellule
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            // Retourner si les chaînes doivent être rassemblées dans un pool global
            return false;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


