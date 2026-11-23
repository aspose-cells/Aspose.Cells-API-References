---
title: "Metered.SetMeteredKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Metered. Définit la clé publique et privée de Metered. Si vous achetez une licence Metered lors du démarrage de l'application, cette API doit être appelée normalement, cela suffit. Cependant, si le téléchargement des données de consommation échoue constamment et dépasse 24 heures, la licence sera mise en statut d'évaluation. Pour éviter ce cas, vous devez vérifier régulièrement le statut de la licence ; si elle est en statut d'évaluation, appelez à nouveau cette API."
type: docs
url: /fr/net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Définit la clé publique et privée mesurée. Si vous achetez une licence à compte, au démarrage de l'application, cette API doit être appelée, normalement cela suffit. Cependant, si le téléchargement des données de consommation échoue constamment et dépasse 24 heures, la licence sera mise en statut d'évaluation ; pour éviter ce cas, vous devez vérifier régulièrement le statut de la licence, et s'il est en statut d'évaluation, appeler à nouveau cette API.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| publicKey | String | clé publique |
| privateKey | String | clé privée |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodSetMeteredKeyWithStringStringDemo
    {
        public static void Run()
        {
            // Définir les clés publiques et privées mesurées
            Metered metered = new Metered();
            metered.SetMeteredKey(
                "asposenet7c90badb00ba4f4bbd35634f4d481c14",
                "FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");

            // Obtenir la quantité de consommation mesurée
            decimal consumption = Metered.GetConsumptionQuantity();
            Console.WriteLine("Consumption quantity: " + consumption);

            // Obtenir le crédit de consommation mesuré
            decimal credit = Metered.GetConsumptionCredit();
            Console.WriteLine("Consumption credit: " + credit);
        }
    }
}
```

### Voir aussi

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


