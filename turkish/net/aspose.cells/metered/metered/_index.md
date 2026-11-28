---
title: "Metered.Metered"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Metered yapıcı. Bu sınıfın yeni bir örneğini başlatır"
type: docs
url: /tr/net/aspose.cells/metered/metered/
---
## Metered constructor

Bu sınıfın yeni bir örneğini başlatır.

```csharp
public Metered()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodCtorDemo
    {
        public static void Run()
        {
            // Yapıcıyı kullanarak bir örnek oluşturun
            Metered metered = new Metered();

            // Metered lisansını ayarlayın
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // İşlevselliği göstermek için basit bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Metered License Demo");
            
            // Çalışma kitabını kaydedin
            workbook.Save("MeteredDemoOutput.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


