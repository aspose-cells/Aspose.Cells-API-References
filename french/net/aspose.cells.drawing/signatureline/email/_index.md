---
title: "SignatureLine.Email"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SignatureLine. Obtient ou définit l'e-mail du signataire"
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/email/
---
## SignatureLine.Email property

Obtient ou définit l'email du chanteur.

```csharp
public string Email { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyEmailDemo
    {
        public static void Run()
        {
            // Créer une nouvelle ligne de signature
            SignatureLine signatureLine = new SignatureLine();
            
            // Définir les propriétés de la ligne de signature, y compris l'e-mail
            signatureLine.Signer = "Simon Zhao";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "Simon.Zhao@aspose.com";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            
            // Afficher la propriété e-mail
            Console.WriteLine("Signer Email: " + signatureLine.Email);
        }
    }
}
```

### Voir aussi

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


