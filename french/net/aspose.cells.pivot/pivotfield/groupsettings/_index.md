---
title: "PivotField.GroupSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient les paramètres de groupe du champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/groupsettings/
---
## PivotField.GroupSettings property

Obtient les paramètres de groupe du champ pivot.

```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```

### Remarques

Si ce champ n’est pas groupé, Null sera retourné.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyGroupSettingsDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Accédez au deuxième champ de base (en supposant qu’il existe)
            if (pivotTable.BaseFields.Count > 1)
            {
                PivotField pivotField = pivotTable.BaseFields[1];
                
                // Vérifiez si le champ possède des paramètres de groupe
                if (pivotField.GroupSettings != null)
                {
                    Console.WriteLine("Field has grouping enabled");
                    Console.WriteLine("Group type: " + pivotField.GroupSettings.Type);
                }
                else
                {
                    Console.WriteLine("Field has no grouping settings");
                }
                
                // Exemple de regroupement d’un champ numérique
                if (pivotField.GroupSettings == null && 
                    pivotField.PivotItems.Count > 0 && 
                    pivotField.PivotItems[0].Value is double)
                {
                    // Regrouper par intervalle numérique (intervalles de 10 unités)
                    pivotField.GroupBy(10.0, false);
                    Console.WriteLine("Field grouped by numeric range");
                }
            }
            
            // Enregistrer le classeur modifié
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


