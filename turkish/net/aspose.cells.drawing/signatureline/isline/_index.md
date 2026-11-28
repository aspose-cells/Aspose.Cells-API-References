---
title: "SignatureLine.IsLine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SignatureLine özelliği. Bunun bir imza satırı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/signatureline/isline/
---
## SignatureLine.IsLine property

Bir imza satırı olup olmadığını gösterir.

```csharp
public bool IsLine { get; set; }
```

### Örnekler

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
            // Bir imza satırı örneği oluştur
            SignatureLine signature = new SignatureLine();
            
            // IsLine değerini true olarak ayarla
            signature.IsLine = true;
            
            // IsLine kullanımını kontrol et ve göster
            if (signature.IsLine)
            {
                Console.WriteLine("Signature line is active.");
            }
            
            // IsLine durumunu değiştir
            signature.IsLine = false;
            
            if (!signature.IsLine)
            {
                Console.WriteLine("Signature line is now inactive.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


