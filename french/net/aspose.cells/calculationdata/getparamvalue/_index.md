---
title: "CalculationData.GetParamValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CalculationData. Obtient l'objet valeur représenté du paramètre à un indice donné"
type: docs
url: /fr/net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

Obtient l'objet valeur représentée du paramètre à un index donné.

```csharp
public object GetParamValue(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice du paramètre (à partir de 0) |

### Valeur de retour

La valeur calculée du paramètre.

### Remarques

Pour un paramètre :

S'il s'agit d'une valeur simple, alors renvoie la valeur simple elle‑même ;

S'il s'agit d'une référence, alors renvoie l'objet ReferredArea ;

S'il fait référence à un ou plusieurs jeux de données contenant plusieurs valeurs, alors renvoie un tableau d'objets ;

S'il s'agit d'une sorte d'expression qui doit être calculée, elle sera calculée en mode valeur et, en général, une seule valeur sera renvoyée selon la base de la cellule actuelle. Par exemple, si un paramètre de la formule de D2 est A:A+B:B, alors A2+B2 sera calculé et renvoyé. Cependant, si ce paramètre a été spécifié en mode tableau (par [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) ou [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), alors un tableau (object[][]) sera renvoyé dont les éléments sont A1+B1,A2+B2,....

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://localhost:9090\", \"Target\")";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new HyperlinkCalculationEngine();
            workbook.CalculateFormula(options);
        }

        class HyperlinkCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName.Equals("HYPERLINK", StringComparison.OrdinalIgnoreCase))
                {
                    Console.WriteLine("URL Parameter: " + data.GetParamValue(0));
                    Console.WriteLine("Display Text: " + data.GetParamValue(1));
                }
            }
        }
    }
}
```

### Voir aussi

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


