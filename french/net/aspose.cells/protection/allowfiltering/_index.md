---
title: "Protection.AllowFiltering"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Représente si l'utilisateur est autorisé à utiliser un AutoFilter qui a été créé avant que la feuille ne soit protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

Représente si l'utilisateur est autorisé à utiliser un AutoFilter créé avant que la feuille ne soit protégée.

```csharp
public bool AllowFiltering { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFilteringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Activer la protection de la feuille
            worksheet.Protect(ProtectionType.All);
            
            // Définir la propriété AllowFiltering sur true
            worksheet.Protection.AllowFiltering = true;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier que la propriété a été enregistrée correctement
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AllowFiltering: " + 
                loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


