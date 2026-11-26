---
title: "Metered.SetMeteredKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Metered. Устанавливает публичный и приватный ключ Metered. Если вы приобретаете лицензию Metered при запуске приложения, этот API обычно должен быть вызван — этого достаточно. Однако если постоянно не удаётся загрузить данные о потреблении и проходит более 24 часов, лицензия будет переведена в статус оценки; чтобы избежать такой ситуации, следует регулярно проверять статус лицензии, и если он находится в статусе оценки, вызвать этот API снова"
type: docs
url: /ru/net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Устанавливает metered public and private key. Если вы приобрели metered‑лицензию, при запуске приложения этот API должен быть вызван, обычно этого достаточно. Однако, если постоянно не удаётся загрузить данные о потреблении и прошло более 24 часов, лицензия будет переведена в статус оценки; чтобы избежать такой ситуации, следует регулярно проверять статус лицензии, и если он находится в статусе оценки, вызвать этот API снова.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| publicKey | String | открытый ключ |
| privateKey | String | закрытый ключ |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodSetMeteredKeyWithStringStringDemo
    {
        public static void Run()
        {
            // Установить измеряемые открытые и закрытые ключи
            Metered metered = new Metered();
            metered.SetMeteredKey(
                "asposenet7c90badb00ba4f4bbd35634f4d481c14",
                "FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");

            // Получить измеряемое количество потребления
            decimal consumption = Metered.GetConsumptionQuantity();
            Console.WriteLine("Consumption quantity: " + consumption);

            // Получить измеряемый кредит потребления
            decimal credit = Metered.GetConsumptionCredit();
            Console.WriteLine("Consumption credit: " + credit);
        }
    }
}
```

### См. также

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


