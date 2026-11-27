---
title: "Metered.GetProductName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Metered method. Hämtar produktnamn"
type: docs
url: /sv/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

Hämtar produktnamn

```csharp
public string GetProductName()
```

### Returvärde

produktnamn

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // Skapa en metered-instans
            Metered metered = new Metered();
            
            // Ställ in metered-nycklar (ersätt med faktiska nycklar)
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Hämta och visa produktnamn
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Demonstrera grundläggande användning med ett enkelt kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### Se även

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


