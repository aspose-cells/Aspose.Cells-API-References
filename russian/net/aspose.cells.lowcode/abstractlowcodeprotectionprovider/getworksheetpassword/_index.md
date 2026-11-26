---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeProtectionProvider. Получает пароль для защиты указанного листа"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

Получает пароль для защиты указанного листа.

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### Возвращаемое значение

Пароль для защиты указанного листа.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // Создайте экземпляр пользовательского провайдера защиты
            var provider = new CustomProtectionProvider();

            try
            {
                // Вызвать GetWorksheetPassword с именем листа
                string password = provider.GetWorksheetPassword(sheetName);

                // Применить защиту к листу, используя полученный пароль
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // Сохранить защищённую книгу
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // Пользовательская реализация, возвращающая пароль на основе имени листа
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // Простая логика генерации пароля для демонстрации
            return $"pw_{sheetName}";
        }
    }
}
```

### См. также

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


