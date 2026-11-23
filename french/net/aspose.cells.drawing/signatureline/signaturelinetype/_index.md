---
title: "SignatureLine.SignatureLineType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SignatureLine. Obtient ou définit le type de signature. Default  Lorsque la valeur par défaut est définie, la valeur correspondante de ProviderId est fixée à 00000000000000000000000000000000. Stamp  Lorsque la valeur est Stamp, la valeur correspondante de ProviderId est généralement 000CD6A400000000C000000000000046. Custom  Lorsque la valeur est Custom, la valeur correspondante de ProviderId doit généralement être définie par l'utilisateur. elle doit être obtenue à partir de la documentation fournie avec le fournisseur"
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

Obtient ou définit le type de signature. Default - Lorsque la valeur par défaut est définie, la valeur correspondante de ProviderId est fixée à {0000000000-0000-0000-0000-0000000000}. Stamp - Lorsque la valeur est Stamp, la valeur correspondante de ProviderId est généralement {000CD6A4-0000-0000-C000-000000000046}. Custom - Lorsque la valeur est Custom, la valeur correspondante de ProviderId doit généralement être définie par l'utilisateur. Elle doit être obtenue à partir de la documentation fournie avec le fournisseur.

```csharp
public SignatureType SignatureLineType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLinePropertySignatureLineTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une ligne de signature
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // Afficher le SignatureLineType actuel
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // Définir SignatureLineType sur Stamp
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // Ajouter la ligne de signature à la feuille de calcul en l'ajoutant aux formes
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // Modifier SignatureLineType en Custom avec un ProviderId personnalisé
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // Enregistrez le classeur
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


