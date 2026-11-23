---
title: "Classe SignatureLine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.SignatureLine. Représente la ligne de signature"
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

Représente la ligne de signature.

```csharp
public class SignatureLine
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SignatureLine](signatureline/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | Indique si des commentaires peuvent être joints. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Obtient ou définit l'email du chanteur. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Obtient ou définit l'identifiant de cette ligne de signature. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | Obtient ou définit le texte affiché à l'utilisateur lors de la signature. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Indique s'il s'agit d'une ligne de signature. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | Obtient ou définit l'ID du fournisseur de signature. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | Indique si la date de signature doit être affichée. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | Obtient ou définit le type de signature. Default - Lorsque la valeur par défaut est définie, la valeur correspondante de ProviderId est fixée à {0000000000-0000-0000-0000-0000000000}. Stamp - Lorsque la valeur est Stamp, la valeur correspondante de ProviderId est généralement {000CD6A4-0000-0000-C000-000000000046}. Custom - Lorsque la valeur est Custom, la valeur correspondante de ProviderId doit généralement être définie par l'utilisateur. Elle doit être obtenue à partir de la documentation fournie avec le fournisseur. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | Obtient ou définit le signataire. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Obtient ou définit le titre du chanteur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLineDemo
    {
        public static void SignatureLineExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajout d'une image
            int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
            Picture pic = worksheet.Pictures[imgIndex];

            // Créer un objet ligne de signature
            SignatureLine s = new SignatureLine();
            s.Signer = "Simon Zhao";
            s.Title = "Development Lead";
            s.Email = "Simon.Zhao@aspose.com";
            s.Id = Guid.NewGuid();
            s.ProviderId = Guid.NewGuid();
            s.IsLine = true;
            s.AllowComments = true;
            s.ShowSignedDate = true;
            s.Instructions = "Just do it.";

            // Attribuer l'objet de ligne de signature à la propriété Picture.SignatureLine
            pic.SignatureLine = s;

            // Enregistrez le fichier Excel
            workbook.Save("SignatureLineExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


