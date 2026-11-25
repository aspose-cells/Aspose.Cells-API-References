---
title: "Metered.SetMeteredKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Metered. Imposta la chiave pubblica e privata di metered. Se acquisti una licenza metered all'avvio dell'applicazione, questa API dovrebbe essere chiamata normalmente; questo è sufficiente. Tuttavia, se fallisce sempre il caricamento dei dati di consumo e supera le 24 ore, la licenza verrà impostata allo stato di valutazione; per evitare tale caso dovresti controllare regolarmente lo stato della licenza e, se è in stato di valutazione, chiamare nuovamente questa API."
type: docs
url: /it/net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Imposta la chiave pubblica e privata metered. Se acquisti una licenza metered, all'avvio dell'applicazione questa API dovrebbe essere chiamata; normalmente è sufficiente. Tuttavia, se il caricamento dei dati di consumo fallisce continuamente e supera le 24 ore, la licenza verrà impostata in stato di valutazione; per evitare tale caso, dovresti controllare regolarmente lo stato della licenza e, se è in stato di valutazione, chiamare nuovamente questa API.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| publicKey | String | chiave pubblica |
| privateKey | String | chiave privata |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodSetMeteredKeyWithStringStringDemo
    {
        public static void Run()
        {
            // Imposta le chiavi pubbliche e private a consumo
            Metered metered = new Metered();
            metered.SetMeteredKey(
                "asposenet7c90badb00ba4f4bbd35634f4d481c14",
                "FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");

            // Ottieni la quantità di consumo misurata
            decimal consumption = Metered.GetConsumptionQuantity();
            Console.WriteLine("Consumption quantity: " + consumption);

            // Ottieni il credito di consumo misurato
            decimal credit = Metered.GetConsumptionCredit();
            Console.WriteLine("Consumption credit: " + credit);
        }
    }
}
```

### Vedi anche

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


