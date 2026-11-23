---
title: "Validation.AddAreas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Validation. Applique la validation aux zones données"
type: docs
url: /fr/net/aspose.cells/validation/addareas/
---
## Validation.AddAreas method

Applique la validation aux zones données.

```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| zones | CellArea[] | Les zones. |
| checkIntersection | Boolean | Vérifier l'intersection de la zone donnée avec les zones des validations existantes. Si une validation a été appliquée dans la zone donnée (ou une partie de celle-ci), alors la validation existante doit d'abord être supprimée de la zone donnée. Sinon, une corruption peut être provoquée pour les validations générées. Si l'utilisateur est sûr que toutes les zones ajoutées n'intersectent aucune zone existante, ce paramètre peut être défini sur false pour des considérations de performance. |
| checkEdge | Boolean | Vérifier le bord des zones appliquées de cette validation. Les paramètres internes de la validation dépendent de la zone en haut à gauche de ses plages appliquées, donc si l'une des zones données devient la nouvelle zone en haut à gauche des plages appliquées, les paramètres internes doivent être modifiés et reconstruits, sinon un résultat inattendu peut survenir. Si l'utilisateur est sûr qu'aucune des zones ajoutées n'est en haut à gauche, ce paramètre peut être défini sur false pour des considérations de performance. |

### Remarques

Dans cette méthode, nous supprimerons toutes les anciennes validations dans la zone donnée. Pour la zone en haut à gauche des plages appliquées de Validation, d'abord son StartRow est le plus petit, ensuite son StartColumn est le plus petit parmi les zones qui ont le même StartRow minimal.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.List;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.Operator = OperatorType.None;
            validation.Formula1 = "1,2,3";
            validation.InCellDropDown = true;

            CellArea[] areas = new CellArea[2];
            areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
            areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };

            try
            {
                validation.AddAreas(areas, true, false);
                Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");

                foreach (CellArea area in validation.Areas)
                {
                    Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding validation areas: {ex.Message}");
            }

            workbook.Save("ValidationAddAreasDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


