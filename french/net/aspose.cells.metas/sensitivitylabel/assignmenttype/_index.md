---
title: "SensitivityLabel.AssignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SensitivityLabel. Obtient et définit la méthode d'affectation du label de sensibilité"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

Obtient et définit la méthode d'affectation pour l'étiquette de sensibilité.

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyAssignmentTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une instance de SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Définir les propriétés de base
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Démontrez l'obtention de la valeur initiale de AssignmentType
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // Définir AssignmentType sur Privileged et afficher le changement
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // Revenir à Standard pour démontrer qu'il est en lecture-écriture
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // Enregistrez le classeur
                workbook.Save("AssignmentTypeDemo.xlsx");
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

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


