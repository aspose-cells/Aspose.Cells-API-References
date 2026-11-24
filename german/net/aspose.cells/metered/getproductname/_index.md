---
title: "Metered.GetProductName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Metered-Methode. Gibt den Produktnamen zurück"
type: docs
url: /de/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

Produktname abrufen

```csharp
public string GetProductName()
```

### Rückgabewert

Produktname

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // Erstelle eine nutzungsbasierte Instanz
            Metered metered = new Metered();
            
            // Setze nutzungsbasierte Schlüssel (ersetze durch echte Schlüssel)
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Abrufen und Anzeigen des Produktnamens
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Demonstriere die grundlegende Verwendung mit einer einfachen Tabelle
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


