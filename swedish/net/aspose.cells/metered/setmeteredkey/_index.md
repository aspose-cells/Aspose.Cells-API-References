---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Metered method. Ställer in metered offentliga och privata nycklar. Om du köper en metered-licens när du startar applikationen bör detta API normalt anropas, det räcker. Men om uppladdning av konsumtionsdata alltid misslyckas och överstiger 24 timmar kommer licensen att sättas till utvärderingsstatus; för att undvika ett sådant fall bör du regelbundet kontrollera licensstatusen och om den är i utvärderingsstatus anropa detta API igen."
type: docs
url: /sv/net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Sätter metered offentlig och privat nyckel. Om du köper en metered-licens, när du startar applikationen bör detta API anropas, normalt räcker detta. Men om uppladdning av förbrukningsdata alltid misslyckas och överstiger 24 timmar, kommer licensen att sättas till utvärderingsstatus. För att undvika detta bör du regelbundet kontrollera licensstatusen, och om den är i utvärderingsstatus, anropa detta API igen.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| publicKey | String | offentlig nyckel |
| privateKey | String | privat nyckel |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodSetMeteredKeyWithStringStringDemo
    {
        public static void Run()
        {
            // Ställ in metered offentliga och privata nycklar
            Metered metered = new Metered();
            metered.SetMeteredKey(
                "asposenet7c90badb00ba4f4bbd35634f4d481c14",
                "FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");

            // Hämta metered konsumtionskvantitet
            decimal consumption = Metered.GetConsumptionQuantity();
            Console.WriteLine("Consumption quantity: " + consumption);

            // Hämta metered konsumtionskredit
            decimal credit = Metered.GetConsumptionCredit();
            Console.WriteLine("Consumption credit: " + credit);
        }
    }
}
```

### Se även

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


