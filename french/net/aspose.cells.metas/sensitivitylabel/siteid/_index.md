---
title: "SensitivityLabel.SiteId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SensitivityLabel. Représente l'identifiant du site Azure Active Directory (Azure AD) correspondant à la stratégie de label de sensibilité qui décrit le label de sensibilité"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Représente l'identifiant du site Azure Active Directory (Azure AD) correspondant à la stratégie d'étiquette de sensibilité qui décrit l'étiquette de sensibilité.

```csharp
public string SiteId { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertySiteIdDemo
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

                // Démontrez l'obtention de la valeur initiale de SiteId
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // Définissez SiteId à un identifiant de site Azure AD d'exemple
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // Modifiez SiteId pour démontrer qu'il est en lecture‑écriture
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // Montrez comment SiteId se rapporte aux autres propriétés
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // Enregistrez le classeur
                workbook.Save("SiteIdDemo.xlsx");
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


