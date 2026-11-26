---
title: "Metered.SetMeteredKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Metered. Establece la clave pública y privada de metered. Si compras una licencia metered al iniciar la aplicación, esta API debe llamarse normalmente; esto es suficiente. Sin embargo, si siempre falla la carga de datos de consumo y supera las 24 horas, la licencia se establecerá en estado de evaluación; para evitar tal caso, deberías comprobar regularmente el estado de la licencia y, si está en estado de evaluación, llamar a esta API nuevamente."
type: docs
url: /es/net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Establece la clave pública y privada medida. Si usted adquiere una licencia medida, al iniciar la aplicación, debe llamarse a esta API; normalmente, eso es suficiente. Sin embargo, si siempre falla la carga de datos de consumo y supera las 24 horas, la licencia se establecerá en estado de evaluación; para evitar tal caso, debe comprobar regularmente el estado de la licencia, y si está en estado de evaluación, llamar a esta API nuevamente.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| publicKey | String | clave pública |
| privateKey | String | clave privada |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodSetMeteredKeyWithStringStringDemo
    {
        public static void Run()
        {
            // Establecer claves públicas y privadas medidas
            Metered metered = new Metered();
            metered.SetMeteredKey(
                "asposenet7c90badb00ba4f4bbd35634f4d481c14",
                "FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");

            // Obtener cantidad de consumo medida
            decimal consumption = Metered.GetConsumptionQuantity();
            Console.WriteLine("Consumption quantity: " + consumption);

            // Obtener crédito de consumo medido
            decimal credit = Metered.GetConsumptionCredit();
            Console.WriteLine("Consumption credit: " + credit);
        }
    }
}
```

### Ver también

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


