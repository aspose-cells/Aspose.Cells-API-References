---
title: "Klasse Metered"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Metered Klasse. Stellt Methoden zum Festlegen des gemessenen Schlüssels bereit"
type: docs
url: /de/net/aspose.cells/metered/
---
## Metered class

Stellt Methoden bereit, um den gemessenen Schlüssel festzulegen.

```csharp
public class Metered
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Metered](metered/)() | Initialisiert eine neue Instanz dieser Klasse. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Produktname abrufen |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Setzt den metered public und private key. Wenn Sie eine metered Lizenz erwerben, sollte diese API beim Start der Anwendung aufgerufen werden; normalerweise reicht das aus. Wenn jedoch ständig das Hochladen von Verbrauchsdaten fehlschlägt und 24 Stunden überschritten werden, wird die Lizenz auf den Evaluierungsstatus gesetzt. Um einen solchen Fall zu vermeiden, sollten Sie regelmäßig den Lizenzstatus prüfen; ist er im Evaluierungsstatus, rufen Sie diese API erneut auf. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Verbrauchsguthaben abrufen |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Verbrauchsdateigröße abrufen |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Prüfen, ob metered lizenziert ist |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredDemo
    {
        public static void MeteredExample()
        {
            // Instanz der Klasse Metered erstellen
            Metered metered = new Metered();

            // Den metered Schlüssel festlegen
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // Produktname abrufen und anzeigen
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Zusätzlicher Code, um zu demonstrieren, wie die Instanz verwendet werden könnte
            // Zum Beispiel ein Arbeitsbuch erstellen und speichern
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


