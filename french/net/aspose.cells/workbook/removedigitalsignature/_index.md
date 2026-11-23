---
title: "Workbook.RemoveDigitalSignature"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Supprime la signature numérique de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/workbook/removedigitalsignature/
---
## Workbook.RemoveDigitalSignature method

Supprime la signature numérique de cette feuille de calcul.

```csharp
public void RemoveDigitalSignature()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveDigitalSignatureDemo
    {
        public static void Run()
        {
            // Créer un classeur avec une signature numérique
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Enregistrer avec une signature numérique (dans un scénario réel, cela serait signé externement)
            string signedPath = "SignedWorkbook.xlsx";
            book.Save(signedPath, SaveFormat.Xlsx);

            // Charger le classeur signé
            Workbook signedBook = new Workbook(signedPath);
            Console.WriteLine("Workbook is digitally signed: " + signedBook.IsDigitallySigned);

            // Supprimer la signature numérique
            signedBook.RemoveDigitalSignature();
            string unsignedPath = "UnsignedWorkbook.xlsx";
            signedBook.Save(unsignedPath);

            // Vérifier que la signature a été supprimée
            Workbook unsignedBook = new Workbook(unsignedPath);
            Console.WriteLine("After removal, workbook is digitally signed: " + unsignedBook.IsDigitallySigned);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


