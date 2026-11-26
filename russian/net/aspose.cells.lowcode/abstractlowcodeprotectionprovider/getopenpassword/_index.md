---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeProtectionProvider. Получает пароль для открытия файла таблицы"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

Получает пароль для открытия файла электронной таблицы.

```csharp
public virtual string GetOpenPassword()
```

### Возвращаемое значение

Пароль для открытия файла таблицы. Пустой означает отсутствие защиты при открытии файла.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // Создать экземпляр поставщика защиты
                var protectionProvider = new DemoProtectionProvider();

                // Вызвать метод GetOpenPassword для получения пароля
                string password = protectionProvider.GetOpenPassword();

                // Создать новую книгу и применить пароль
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // Сохранить книгу, защищённую паролем
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### См. также

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


