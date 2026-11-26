---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeProtectionProvider. Получает пароль для изменения файла электронной таблицы"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

Получает пароль для изменения файла электронной таблицы.

```csharp
public virtual string GetWritePassword()
```

### Возвращаемое значение

Пароль для изменения файла электронной таблицы. Пустой означает отсутствие защиты при изменении файла.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Создайте экземпляр пользовательского провайдера защиты
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // Явно вызвать GetWritePassword и отобразить результат
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // Сохранить книгу — напрямую применить защиту от записи
                workbook.Settings.WriteProtection.Password = writePassword;
                workbook.Save("MethodGetWritePasswordDemo.xlsx");
                Console.WriteLine("Workbook saved with write protection password.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
            }
        }

    }

    // Реализация пользовательского поставщика защиты
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // Реализовать другие необходимые методы с возвратом значений по умолчанию
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### См. также

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


