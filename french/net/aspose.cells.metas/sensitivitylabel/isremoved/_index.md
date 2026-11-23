---
title: "SensitivityLabel.IsRemoved"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SensitivityLabel. Indique si le label de sensibilité a été supprimé"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

Indique si l'étiquette de sensibilité a été supprimée.

```csharp
public bool IsRemoved { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsRemovedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une instance de label de sensibilité via la réflexion
                // car l'instanciation directe n'est pas disponible
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Définissez les propriétés requises
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // Affichez la valeur initiale de IsRemoved
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // Démontrez la définition de la propriété IsRemoved (car elle est en lecture‑écriture)
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // Basculez la valeur pour montrer qu'elle peut être modifiée
                label.IsRemoved = false;
                Console.WriteLine("Final IsRemoved value: " + label.IsRemoved);
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


