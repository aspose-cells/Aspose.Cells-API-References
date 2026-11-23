---
title: "SensitivityLabel.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SensitivityLabel. Obtient et définit l'ID de l'étiquette de sensibilité"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

Obtient et définit l'ID de l'étiquette de sensibilité.

```csharp
public string Id { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une instance de SensitivityLabel
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Démontrer la définition et la récupération de la propriété Id
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // Afficher la valeur de l'ID
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // Modifiez la valeur Id pour démontrer qu'elle est en lecture‑écriture
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // Montrez que la propriété affecte d'autres opérations
                label.IsEnabled = true;
                Console.WriteLine($"Label {label.Id} is enabled: {label.IsEnabled}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


