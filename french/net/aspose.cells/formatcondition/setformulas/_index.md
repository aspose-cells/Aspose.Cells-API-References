---
title: "FormatCondition.SetFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatCondition. Définit la valeur ou l'expression associée à cette condition de formatage"
type: docs
url: /fr/net/aspose.cells/formatcondition/setformulas/
---
## FormatCondition.SetFormulas method

Définit la valeur ou l'expression associée à cette condition de format.

```csharp
public void SetFormulas(string formula1, string formula2, bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formula1 | String | La valeur ou l'expression associée à cette condition de formatage. Si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon elle sera considérée comme une valeur simple (texte, nombre, bool). Pour une valeur texte qui commence par '=', l'utilisateur peut la saisir comme formule au format : \"=\\\"=...\\\"\". |
| formula2 | String | La valeur ou l'expression associée à cette condition de format. Le format d'entrée est le même que formula1 |
| isR1C1 | Boolean | Indique si la formule est une formule R1C1. |
| isLocal | Boolean | Si la formule est formatée selon la locale. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionMethodSetFormulasWithStringStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int formatIndex = cfs.Add();
            FormatConditionCollection fcs = cfs[formatIndex];
            
            fcs.AddArea(CellArea.CreateCellArea("A1", "C10"));
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcs[conditionIndex];
            
            fc.Operator = OperatorType.Between;
            fc.SetFormulas("=1", "=2", false, false);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


