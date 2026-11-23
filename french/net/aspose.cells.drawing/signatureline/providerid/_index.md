---
title: "SignatureLine.ProviderId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SignatureLine. Obtient ou définit l'ID du fournisseur de signature"
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

Obtient ou définit l'ID du fournisseur de signature.

```csharp
public Guid ProviderId { get; set; }
```

### Remarques

Il s'agit généralement du CLSID du module COM du fournisseur.

### Exemples

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Créer une nouvelle ligne de signature
            SignatureLine signatureLine = new SignatureLine();
            
            // Définir les propriétés de la ligne de signature
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";
            signatureLine.IsLine = true;
            
            // Définir l'ID du fournisseur (exemple de GUID - doit être remplacé par le GUID réel du fournisseur)
            signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
            
            // Définir le type de signature (cela doit correspondre à l'ID du fournisseur)
            signatureLine.SignatureLineType = SignatureType.Stamp;
            
            // Afficher l'ID du fournisseur pour démontrer l'utilisation
            Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
        }
    }
}
```

### Voir aussi

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


