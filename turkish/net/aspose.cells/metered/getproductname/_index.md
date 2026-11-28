---
title: "Metered.GetProductName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Metered yöntemi. Ürün adını alır"
type: docs
url: /tr/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

Ürün adını alır

```csharp
public string GetProductName()
```

### Dönüş Değeri

ürün adı

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // Bir metered örneği oluşturun
            Metered metered = new Metered();
            
            // Metered anahtarlarını ayarlayın (gerçek anahtarlarla değiştirin)
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Ürün adını al ve göster
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Basit bir elektronik tabloyla temel kullanımı gösterin
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


