---
title: "AutoFilter.AddIconFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Ajoute un filtre d'icône"
type: docs
url: /fr/net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

Ajoute un filtre d'icône.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| iconSetType | IconSetType | Le type d'ensemble d'icônes. |
| iconId | Int32 | L'identifiant de l'icône. |

### Remarques

Ne prend en charge que l'ajout du filtre d'icône. Ne prend pas en charge la vérification de la visibilité des lignes si le filtre est un filtre d'icône.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir des données d'exemple dans la colonne A
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);
            cell = worksheet.Cells["B1"];
            cell.PutValue("Values2");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(1, 0, 5, 1));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];

            // Obtenir l'instance du filtre automatique
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Définir la plage du filtre automatique (A1:A6) en utilisant startRow, startColumn, endRow
            autoFilter.SetRange(0, 0, 1);

            try
            {
                // Ajouter un filtre d'icône à la première colonne (fieldIndex: 0)
                // Utilisation du jeu d'icônes 3 Feux de circulation (IconSetType.TrafficLights31)
                // Filtrage pour la première icône de l'ensemble (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // Actualiser le filtre pour appliquer les modifications
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


