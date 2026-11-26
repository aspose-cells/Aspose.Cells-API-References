---
title: "Metered.GetConsumptionCredit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Metered. Получает кредит потребления"
type: docs
url: /ru/net/aspose.cells/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Получает кредит потребления

```csharp
public static decimal GetConsumptionCredit()
```

### Возвращаемое значение

количество потребления

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionCreditDemo
    {
        public static void Run()
        {
            // Создать экземпляр класса Metered
            Metered metered = new Metered();

            try
            {
                // Вызвать метод GetConsumptionCredit как статический
                decimal consumptionCredit = Metered.GetConsumptionCredit();
                
                // Отобразить результат
                Console.WriteLine($"Current consumption credit: {consumptionCredit}");
                
                // Создать простую рабочую книгу для демонстрации эффекта (хотя GetConsumptionCredit не изменяет рабочую книгу)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Добавить информацию о кредите потребления в лист
                worksheet.Cells["A1"].PutValue("Consumption Credit:");
                worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
                
                // Сохраните книгу
                workbook.Save("MeteredGetConsumptionCreditDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error getting consumption credit: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


