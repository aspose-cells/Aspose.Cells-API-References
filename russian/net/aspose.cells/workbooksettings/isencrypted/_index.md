---
title: "WorkbookSettings.IsEncrypted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Возвращает значение, указывающее, требуется ли пароль для открытия этой книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/isencrypted/
---
## WorkbookSettings.IsEncrypted property

Получает значение, указывающее, требуется ли пароль для открытия этой рабочей книги.

```csharp
public bool IsEncrypted { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Пример 1: Проверить, зашифрована ли книга, защищённая паролем
            string encryptedFilePath = "encrypted.xlsx";
            var encryptedWorkbook = new Workbook(encryptedFilePath, new LoadOptions { Password = "password" });
            Console.WriteLine($"Encrypted workbook IsEncrypted: {encryptedWorkbook.Settings.IsEncrypted}");

            // Пример 2: Проверить, зашифрована ли обычная книга
            string normalFilePath = "normal.xlsx";
            var normalWorkbook = new Workbook(normalFilePath);
            Console.WriteLine($"Normal workbook IsEncrypted: {normalWorkbook.Settings.IsEncrypted}");

            // Пример 3: Создать и сохранить зашифрованную книгу
            var newWorkbook = new Workbook();
            newWorkbook.Settings.Password = "12345";
            newWorkbook.Save("new_encrypted.xlsx");
            Console.WriteLine($"New workbook IsEncrypted: {newWorkbook.Settings.IsEncrypted}");
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


