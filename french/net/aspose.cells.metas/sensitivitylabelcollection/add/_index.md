---
title: "SensitivityLabelCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SensitivityLabelCollection. Ajoute un label de sensibilité"
type: docs
url: /fr/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

Ajoute un label de sensibilité.

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| id | String | L'ID du label. |
| isEnabled | Boolean | Indique si ce label de sensibilité est activé. |
| methodType | SensitivityLabelAssignmentType | Le type de méthode d'affectation. |
| siteId | String | L'ID du site. |
| markType | SensitivityLabelMarkType | Le type de marque. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelCollectionMethodAddWithStringBooleanSensitivityLabelADemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une nouvelle SensitivityLabelCollection
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // Appeler la méthode Add avec des paramètres spécifiques
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // Ajouter des données pour démontrer l'effet
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


