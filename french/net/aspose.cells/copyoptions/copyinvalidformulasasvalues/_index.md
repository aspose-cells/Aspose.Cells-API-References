---
title: "CopyOptions.CopyInvalidFormulasAsValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CopyOptions. Si la formule n'est pas valide pour la destination, copier uniquement les valeurs."
type: docs
url: /fr/net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

Si la formule n'est pas valide pour la destination cible, seules les valeurs sont copiées.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
    {
        public static void Run()
        {
            // Créer un classeur source avec une feuille de calcul d'exemple
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Ajouter une formule qui pourrait être invalide dans certains contextes
            srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
            srcSheet.Cells["A2"].Value = "Valid Data";

            // Créer un classeur de destination
            Workbook destWorkbook = new Workbook();
            
            // Définir les options de copie pour convertir les formules invalides en valeurs
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            // Copier la feuille de calcul avec les options
            destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);

            // Vérifier les résultats
            Console.WriteLine("A1 (invalid formula copied as value): " + 
                destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
            Console.WriteLine("A2 (valid data): " + 
                destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


