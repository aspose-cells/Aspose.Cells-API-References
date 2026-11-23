---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Worksheet method. Convertit le style de référence de la formule"
type: docs
url: /fr/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

Convertit le style de référence de la formule.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La formule à convertir. |
| toR1C1 | Boolean | Quel style de référence utiliser pour convertir la formule. Si la formule originale est de style de référence A1, alors cette valeur doit être vraie afin que la formule soit convertie du style A1 au style R1C1 ; Si la formule originale est de style de référence R1C1, alors cette valeur doit être fausse afin que la formule soit convertie du style R1C1 au style A1 ; |
| baseCellRow | Int32 | L'index de ligne de la cellule de base. |
| baseCellColumn | Int32 | L'index de colonne de la cellule de base. |

### Valeur de retour

La formule convertie.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Exemple 1 : Convertir le style R1C1 en style A1
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // Exemple 2 : Convertir avec des références mixtes
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


