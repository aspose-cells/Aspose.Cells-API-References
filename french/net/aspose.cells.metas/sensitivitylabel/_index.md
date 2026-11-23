---
title: "Classe SensitivityLabel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Metas.SensitivityLabel class. Représente l'étiquette de sensibilité"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

Représente l'étiquette de sensibilité.

```csharp
public class SensitivityLabel
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | Obtient et définit la méthode d'affectation pour l'étiquette de sensibilité. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | Obtient et définit les types de marquage de contenu qui doivent être appliqués à un fichier. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | Obtient et définit l'ID de l'étiquette de sensibilité. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | Indique si l'étiquette de sensibilité est activée |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | Indique si l'étiquette de sensibilité a été supprimée. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | Représente l'identifiant du site Azure Active Directory (Azure AD) correspondant à la stratégie d'étiquette de sensibilité qui décrit l'étiquette de sensibilité. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Créer une instance de la classe SensitivityLabel en utilisant la réflexion
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Définir les propriétés de base
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // Afficher les valeurs des propriétés
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // Enregistrez le classeur
                workbook.Save("SensitivityLabelDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SensitivityLabel: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


