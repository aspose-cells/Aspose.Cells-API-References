---
title: "PivotTable.GetChildren"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Obtient les tableaux croisés dynamiques enfants qui utilisent ces données de tableau croisé dynamique comme source de données"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/getchildren/
---
## PivotTable.GetChildren method

Obtient les tables de pivot enfants qui utilisent ces données de PivotTable comme source de données.

```csharp
[Obsolete("Use PivotTable.GetDependentPivotTables() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotTable[] GetChildren()
```

### Valeur de retour

l'objet tableau PivotTable

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.GetDependentPivotTables(). Cette méthode sera supprimée 12 mois plus tard à compter d’avril 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetChildrenDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // Créer la table de pivot principale
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "MainPivotTable");
            PivotTable mainPivotTable = pivotTables[index];
            mainPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            mainPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Créer une table de pivot enfant
            index = pivotTables.Add("A1:B4", "E10", "ChildPivotTable");
            PivotTable childPivotTable = pivotTables[index];
            childPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            childPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Établir une relation en partageant les champs de base
            foreach (PivotField field in mainPivotTable.BaseFields)
            {
                childPivotTable.BaseFields.Add(field);
            }

            // Démontrer la méthode GetChildren()
            Console.WriteLine("Child Pivot Tables:");
            foreach (PivotTable child in mainPivotTable.GetChildren())
            {
                Console.WriteLine("Child Pivot Table Name: " + child.Name);
                Console.WriteLine("Child Pivot Table Location: " + child.TableRange1);
            }
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


