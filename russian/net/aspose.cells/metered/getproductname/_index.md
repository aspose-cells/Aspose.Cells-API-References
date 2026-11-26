---
title: "Metered.GetProductName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Metered. Получает название продукта"
type: docs
url: /ru/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

Получает название продукта

```csharp
public string GetProductName()
```

### Возвращаемое значение

название продукта

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // Создать экземпляр Metered
            Metered metered = new Metered();
            
            // Установить ключи Metered (заменить реальными ключами)
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Получить и отобразить название продукта
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Продемонстрировать базовое использование с простой таблицей
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### См. также

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


