---
title: "Metered.GetProductName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Metered. Ottiene il nome del prodotto"
type: docs
url: /it/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

Ottiene il nome del prodotto

```csharp
public string GetProductName()
```

### Valore di ritorno

nome del prodotto

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // Crea un'istanza metered
            Metered metered = new Metered();
            
            // Imposta le chiavi metered (sostituisci con le chiavi effettive)
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Ottieni e visualizza il nome del prodotto
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Dimostra l'uso di base con un semplice foglio di calcolo
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


