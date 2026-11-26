---
title: "Metered.IsMeteredLicensed"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Metered. Проверить, лицензирована ли Metered"
type: docs
url: /ru/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

Проверьте, лицензирован ли metered

```csharp
public static bool IsMeteredLicensed()
```

### Возвращаемое значение

Истина или ложь

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр Metered
            Metered metered = new Metered();

            try
            {
                // Проверить, применена ли лицензия Metered
                bool isLicensed = Metered.IsMeteredLicensed();

                // Отобразить результат
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // Добавить результат в лист
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### См. также

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


