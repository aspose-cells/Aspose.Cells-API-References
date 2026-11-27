---
title: "Klass Metered"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Metered-klass. Tillhandahåller metoder för att ange metered-nyckel"
type: docs
url: /sv/net/aspose.cells/metered/
---
## Metered class

Tillhandahåller metoder för att ställa in mätad nyckel.

```csharp
public class Metered
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Metered](metered/)() | Initierar en ny instans av denna klass. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Hämtar produktnamn |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Sätter metered offentlig och privat nyckel. Om du köper en metered-licens, när du startar applikationen bör detta API anropas, normalt räcker detta. Men om uppladdning av förbrukningsdata alltid misslyckas och överstiger 24 timmar, kommer licensen att sättas till utvärderingsstatus. För att undvika detta bör du regelbundet kontrollera licensstatusen, och om den är i utvärderingsstatus, anropa detta API igen. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Hämtar förbrukningskredit |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Hämtar förbrukningsfilens storlek |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Kontrollera om metered är licensierad |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredDemo
    {
        public static void MeteredExample()
        {
            // Skapa en instans av Metered-klassen
            Metered metered = new Metered();

            // Ställ in den metered-nyckeln
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // Hämta och visa produktnamnet
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Ytterligare kod för att demonstrera hur instansen kan användas
            // Till exempel, skapa en arbetsbok och spara den
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


