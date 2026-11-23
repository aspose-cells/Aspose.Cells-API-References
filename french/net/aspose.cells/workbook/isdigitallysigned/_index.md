---
title: "Workbook.IsDigitallySigned"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Indique si cette feuille de calcul est signée numériquement"
type: docs
url: /fr/net/aspose.cells/workbook/isdigitallysigned/
---
## Workbook.IsDigitallySigned property

Indique si cette feuille de calcul est signée numériquement.

```csharp
public bool IsDigitallySigned { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsDigitallySignedDemo
    {
        public static void Run()
        {
            // Charger un classeur signé numériquement
            Workbook book = new Workbook("Test_DigiSign.xlsx");
            
            // Vérifier si le classeur est signé numériquement
            bool isSigned = book.IsDigitallySigned;
            Console.WriteLine("Workbook is digitally signed: " + isSigned);

            if (isSigned)
            {
                // Enregistrer une copie (la signature sera préservée)
                book.Save("SignedCopy.xlsx");
                
                // Supprimer la signature numérique
                book.RemoveDigitalSignature();
                book.Save("UnsignedCopy.xlsx");
                
                // Vérifier que la signature a été supprimée
                Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
                Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


