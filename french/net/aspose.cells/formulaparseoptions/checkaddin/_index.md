---
title: "FormulaParseOptions.CheckAddIn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaParseOptions. Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. La valeur par défaut est true. Si la fonction définie par l'utilisateur correspond à un complément présent dans les liens externes existants, elle sera considérée comme ce complément"
type: docs
url: /fr/net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Indique s'il faut vérifier les compléments dans les liens externes existants du classeur actuel pour les fonctions définies par l'utilisateur sans lien externe. La valeur par défaut est true (si la fonction définie par l'utilisateur correspond à un complément dans les liens externes existants, alors il est considéré comme le complément).

```csharp
public bool CheckAddIn { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCheckAddInDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Enregistrer une fonction d'add-in
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);

            // Sans CheckAddIn=false - la formule sera convertie au format add-in
            cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);

            // Avec CheckAddIn=false - la formule reste inchangée
            cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
            Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
        }
    }
}
```

### Voir aussi

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


