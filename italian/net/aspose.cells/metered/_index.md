---
title: "Classe Metered"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Metered. Fornisce metodi per impostare la chiave metered"
type: docs
url: /it/net/aspose.cells/metered/
---
## Metered class

Fornisce metodi per impostare la chiave a consumo.

```csharp
public class Metered
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Metered](metered/)() | Inizializza una nuova istanza di questa classe. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Ottiene il nome del prodotto |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Imposta la chiave pubblica e privata metered. Se acquisti una licenza metered, all'avvio dell'applicazione questa API dovrebbe essere chiamata; normalmente è sufficiente. Tuttavia, se il caricamento dei dati di consumo fallisce continuamente e supera le 24 ore, la licenza verrà impostata in stato di valutazione; per evitare tale caso, dovresti controllare regolarmente lo stato della licenza e, se è in stato di valutazione, chiamare nuovamente questa API. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Ottiene il credito di consumo |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Ottiene la dimensione del file di consumo |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Verifica se Metered è licenziato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredDemo
    {
        public static void MeteredExample()
        {
            // Crea un'istanza della classe Metered
            Metered metered = new Metered();

            // Imposta la chiave metered
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // Ottieni e visualizza il nome del prodotto
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Codice aggiuntivo per dimostrare come l'istanza potrebbe essere utilizzata
            // Ad esempio, creando una cartella di lavoro e salvandola
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


