---
title: "CalculationOptions.CharacterEncoding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. Spécifie l'encodage utilisé pour l'encodage/décodage des caractères lors du calcul des formules. Pour des fonctions telles que CHAR CODE, le résultat calculé dépend des paramètres régionaux et du jeu de caractères par défaut de l'environnement. Avec cette propriété, l'utilisateur peut spécifier l'encodage approprié utilisé pour ces fonctions afin d'obtenir le résultat attendu"
type: docs
url: /fr/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

Spécifie l'encodage utilisé pour encoder/décoder les caractères lors du calcul des formules. Pour des fonctions telles que CHAR, CODE, le résultat calculé dépend des paramètres régionaux et du jeu de caractères par défaut de l'environnement. Avec cette propriété, l'utilisateur peut spécifier l'encodage approprié utilisé par ces fonctions pour obtenir le résultat attendu.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


