---
title: "Cell.GetFormatConditions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient les conditions de format qui s'appliquent à cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Obtient les conditions de format qui s'appliquent à cette cellule.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Valeur de retour

Renvoie l'objet [`FormatConditionCollection`](../../formatconditioncollection/)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormatConditionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la collection de cellules
            Cells cells = worksheet.Cells;
            
            // Ajoutez des données d'exemple
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            
            // Ajouter une condition de format à la cellule A1
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            
            // Obtenir les conditions de format pour la cellule A1
            FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
            
            // Afficher le nombre de conditions de format
            Console.WriteLine("Number of format conditions: " + conditions.Length);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


