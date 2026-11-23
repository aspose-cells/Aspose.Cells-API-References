---
title: "Énumération SignatureType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.SignatureType. Spécifie le type de signature"
type: docs
url: /fr/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

Spécifie le type de signature.

```csharp
public enum SignatureType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | La valeur par défaut, la valeur ProviderId correspondante est fixée à {0000000000-0000-0000-0000-0000000000}. |
| Stamp | `1` | La valeur ProviderId correspondante est généralement {000CD6A4-0000-0000-C000-000000000046}. |
| Custom | `3` | La valeur ProviderId correspondante doit généralement être définie par l'utilisateur. Elle doit être obtenue à partir de la documentation fournie avec le fournisseur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassSignatureTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des lignes de signature avec différents types
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // Enregistrer le classeur avec les configurations de signature
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


