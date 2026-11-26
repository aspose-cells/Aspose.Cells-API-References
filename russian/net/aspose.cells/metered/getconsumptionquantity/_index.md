---
title: "Metered.GetConsumptionQuantity"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Metered. Получает размер файла потребления"
type: docs
url: /ru/net/aspose.cells/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Получает размер файла потребления

```csharp
public static decimal GetConsumptionQuantity()
```

### Возвращаемое значение

количество потребления

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionQuantityDemo
    {
        public static void Run()
        {
            // Создать экземпляр Metered
            Metered metered = new Metered();

            try
            {
                // Установить измеряемые ключи (замените реальными ключами при реальном использовании)
                metered.SetMeteredKey("your-public-key", "your-private-key");

                // Получить количество потребления
                decimal consumptionQuantity = Metered.GetConsumptionQuantity();

                // Отобразить результат
                Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");

                // Создать рабочую книгу для демонстрации измеряемого использования
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Добавить данные, чтобы показать, что рабочая книга функционирует
                worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
                worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");

                // Сохраните книгу
                workbook.Save("MeteredConsumptionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in metered operation: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


