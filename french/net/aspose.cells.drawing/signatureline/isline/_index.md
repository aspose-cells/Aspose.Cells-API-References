---
title: "SignatureLine.IsLine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SignatureLine. Indique s'il s'agit d'une ligne de signature"
type: docs
url: /fr/net/aspose.cells.drawing/signatureline/isline/
---
## SignatureLine.IsLine property

Indique s'il s'agit d'une ligne de signature.

```csharp
public bool IsLine { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIsLineDemo
    {
        public static void Run()
        {
            // Créer une instance de ligne de signature
            SignatureLine signature = new SignatureLine();
            
            // Définir IsLine sur vrai
            signature.IsLine = true;
            
            // Vérifier et démontrer l'utilisation de IsLine
            if (signature.IsLine)
            {
                Console.WriteLine("Signature line is active.");
            }
            
            // Basculer l'état de IsLine
            signature.IsLine = false;
            
            if (!signature.IsLine)
            {
                Console.WriteLine("Signature line is now inactive.");
            }
        }
    }
}
```

### Voir aussi

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


