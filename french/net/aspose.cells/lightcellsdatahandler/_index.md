---
title: "Interface LightCellsDataHandler"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.LightCellsDataHandler. Représente le gestionnaire de données de cellules pour la lecture de gros fichiers de feuilles de calcul en mode léger."
type: docs
url: /fr/net/aspose.cells/lightcellsdatahandler/
---
## LightCellsDataHandler interface

Représente le gestionnaire de données de cellules pour la lecture de grands fichiers de feuille de calcul en mode léger.

```csharp
public interface LightCellsDataHandler
```

## Méthodes

| Nom | Description |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | Commence à traiter une cellule. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | Commence à traiter une ligne. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | Prépare le traitement d’une cellule. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | Prépare le traitement d’une ligne. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | Commence à traiter une feuille de calcul. |

### Remarques

Lors de la lecture d’un classeur avec ce mode, [`StartSheet`](./startsheet/) sera vérifié lors de la lecture de chaque feuille de calcul du classeur. Pour une feuille, si [`StartSheet`](./startsheet/) renvoie true, alors toutes les données et propriétés des lignes/cellules de cette feuille seront vérifiées et traitées par l’implémentation de cette interface. Pour chaque ligne, [`StartRow`](./startrow/) sera appelé pour vérifier si elle doit être traitée. Si une ligne doit être traitée, ses propriétés seront lues en premier et l’utilisateur peut y accéder via [`ProcessRow`](./processrow/). Si les cellules de la ligne doivent également être traitées, alors [`ProcessRow`](./processrow/) doit renvoyer true et ensuite [`StartCell`](./startcell/) sera appelé pour chaque cellule existante de cette ligne afin de vérifier si une cellule doit être traitée. Si une cellule doit être traitée, alors [`ProcessCell`](./processcell/) sera appelé pour la traiter selon l’implémentation de cette interface.  Veuillez noter que l’utilisateur ne doit manipuler que les valeurs et propriétés de l’objet Row/Cell actuel fourni par la méthode correspondante. Comme les données des cellules sont lues depuis le fichier modèle de manière flux, la plupart des autres objets peuvent être réinitialisés/mis à jour plus tard après le chargement des données des cellules. Ainsi, lorsque l’utilisateur manipule d’autres objets dans cette implémentation, ces opérations peuvent ne pas affecter les objets existants dans le classeur. Pire encore, ces opérations peuvent entraîner des données incohérentes dans le classeur et provoquer ensuite des problèmes ou exceptions inattendus. Par conséquent, pour tous les autres objets tels que les formes, la largeur des colonnes et les styles, les mises en forme conditionnelles, ...etc., veuillez ne pas les manipuler dans les méthodes de cette implémentation. Gérez‑les plutôt après la construction du classeur.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerDemo : LightCellsDataHandler
    {
        public static void LightCellsDataHandlerExample()
        {
            // Créer un classeur et le charger avec LightCellsDataHandler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de LightCellsDataHandlerDemo
            LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();

            // Définir le LightCellsDataHandler pour le classeur
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = handler;

            // Chargez le classeur avec les options de chargement spécifiées
            workbook = new Workbook("LargeFile_original.xlsx", loadOptions);

            // Enregistrer le classeur pour démontrer le processus
            workbook.Save("ProcessedLargeFile.xlsx");
        }

        // Implémenter la méthode StartSheet
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine("Starting to process sheet: " + sheet.Name);
            return true; // Continue processing
        }

        // Implémenter la méthode StartRow
        public bool StartRow(int rowIndex)
        {
            Console.WriteLine("Starting to process row: " + rowIndex);
            return true; // Continue processing
        }

        // Implémenter la méthode ProcessRow
        public bool ProcessRow(Row row)
        {
            Console.WriteLine("Processing row: " + row.Index);
            return true; // Continue processing
        }

        // Implémenter la méthode StartCell
        public bool StartCell(int columnIndex)
        {
            Console.WriteLine("Starting to process cell in column: " + columnIndex);
            return true; // Continue processing
        }

        // Implémenter la méthode ProcessCell
        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
            return true; // Continue processing
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


