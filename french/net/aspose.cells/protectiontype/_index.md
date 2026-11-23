---
title: "Enum ProtectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ProtectionType enum. Représente le type de protection du classeur/feuille de calcul"
type: docs
url: /fr/net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

Représente le type de protection du classeur/feuille de calcul.

```csharp
public enum ProtectionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| All | `0` | Représente la protection de tout. |
| Contents | `1` | Représente la protection du contenu, utilisé dans la protection de la feuille de calcul. |
| Objects | `2` | Représente la protection des objets, utilisé dans la protection de la feuille de calcul. |
| Scenarios | `3` | Représente la protection des scénarios, utilisé dans la protection de la feuille de calcul. |
| Structure | `4` | Représente la protection de la structure, utilisé dans la protection du classeur. |
| Windows | `5` | Représente la protection de la fenêtre, utilisé dans la protection du classeur. |
| None | `6` | Représente aucune protection. Uniquement pour la propriété Reading. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Protégez la feuille de calcul avec tous les types de protection
            worksheet.Protect(ProtectionType.All);
            
            // Démontrez l'accès aux propriétés de protection
            Console.WriteLine("Worksheet protection settings:");
            Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
            Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
            Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
            Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
            Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
            Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
            Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
            Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
            Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
            
            // Déprotégez la feuille de calcul
            worksheet.Unprotect();
            
            // Protégez avec des types de protection spécifiques
            worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
            Console.WriteLine("\nWorksheet protected with Contents and Objects only");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


