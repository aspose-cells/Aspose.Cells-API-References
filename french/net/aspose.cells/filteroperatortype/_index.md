---
title: "Enum FilterOperatorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.FilterOperatorType. Type d'opérateur de filtre personnalisé"
type: docs
url: /fr/net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

Type d'opérateur de filtre personnalisé.

```csharp
public enum FilterOperatorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| LessOrEqual | `0` | Représente l'opérateur LessOrEqual. |
| LessThan | `1` | Représente l'opérateur LessThan. |
| Equal | `2` | Représente l'opérateur Equal. |
| GreaterThan | `3` | Représente l'opérateur GreaterThan. |
| NotEqual | `4` | Représente l'opérateur NotEqual. |
| GreaterOrEqual | `5` | Représente l'opérateur GreaterOrEqual. |
| None | `6` | Représente aucune comparaison. |
| BeginsWith | `7` | Commence par le texte. |
| EndsWith | `8` | Se termine par le texte. |
| Contains | `9` | Contient le texte. |
| NotContains | `10` | Ne contient pas le texte. |
| NotBeginsWith | `11` | Ne commence pas par le texte. |
| NotEndsWith | `12` | Ne se termine pas par le texte. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("Bob");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bobby");
            worksheet.Cells["A5"].PutValue("Tom");
            
            // Définir la plage du filtre automatique
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Appliquer un filtre personnalisé pour afficher les noms commençant par "Bo"
            worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
            
            // Actualiser le filtre
            worksheet.AutoFilter.Refresh();
            
            // Enregistrez le classeur
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


