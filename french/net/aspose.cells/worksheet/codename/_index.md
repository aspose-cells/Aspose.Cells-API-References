---
title: "Worksheet.CodeName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient le nom de code de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Obtient le nom de code de la feuille de calcul.

```csharp
public string CodeName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCodeNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Afficher le CodeName par défaut
            Console.WriteLine("Default CodeName: " + worksheet.CodeName);
            
            // Modifier le CodeName
            worksheet.CodeName = "MySheet";
            Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
            
            // Ajouter une nouvelle feuille de calcul et afficher son CodeName
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
            
            // Enregistrez le classeur
            workbook.Save("WorksheetCodeNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


