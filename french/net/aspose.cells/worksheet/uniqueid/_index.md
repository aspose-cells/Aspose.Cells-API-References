---
title: "Worksheet.UniqueId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient et définit l'identifiant unique, identique à 15DB5C3CA5A148AF8F253D86AC232D4F"
type: docs
url: /fr/net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

Obtient et définit l'ID unique, il est identique à {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```csharp
public string UniqueId { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyUniqueIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Générer un identifiant unique pour la feuille de calcul
            string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
            
            // Définir la propriété UniqueId de la première feuille de calcul
            workbook.Worksheets[0].UniqueId = uniqueId;
            
            // Enregistrez le classeur
            string outputPath = "SheetUniqueIdDemo.xlsx";
            workbook.Save(outputPath);
            
            // Recharger le classeur pour vérifier que l'UniqueId persiste
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Afficher l'UniqueId pour démontrer la fonctionnalité
            Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


