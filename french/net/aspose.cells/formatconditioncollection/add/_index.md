---
title: "FormatConditionCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatConditionCollection. Ajoute une condition de formatage et la plage de cellules affectée aux FormatConditions. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels. Les références aux autres feuilles ne sont pas autorisées dans les formules du formatage conditionnel"
type: docs
url: /fr/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Ajoute une condition de formatage et la plage de cellules affectée aux FormatConditions. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels. Les références aux autres feuilles ne sont pas autorisées dans les formules du formatage conditionnel.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Plage de cellules formatées conditionnellement. |
| type | FormatConditionType | Type de mise en forme conditionnelle.It pourrait être l'un des membres de FormatConditionType. |
| operatorType | OperatorType | Opérateur de comparaison.It pourrait être l'un des membres de OperatorType. |
| formula1 | String | La valeur ou l'expression associée à la mise en forme conditionnelle. |
| formula2 | String | La valeur ou l'expression associée à la mise en forme conditionnelle |

### Valeur de retour

[0]:Formatting condition object index;[1] Effected cell rang index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddWithCellAreaFormatConditionTypeOpeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Remplissez des données d'exemple
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Ajouter une mise en forme conditionnelle
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            
            // Démontrer la méthode Add avec les paramètres spécifiés
            fcc.Add(
                CellArea.CreateCellArea(0, 0, 4, 0),
                FormatConditionType.Expression,
                OperatorType.None,
                "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
                null
            );

            // Appliquer la mise en forme
            int fontSize = wb.DefaultStyle.Font.Size;
            fcc[0].Style.Font.Size = fontSize + 2;

            // Enregistrer le classeur pour démontrer le résultat
            wb.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


