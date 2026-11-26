---
title: "Класс WriteProtection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WriteProtection. Указывает настройки защиты от записи для рабочей книги"
type: docs
url: /ru/net/aspose.cells/writeprotection/
---
## WriteProtection class

Указывает параметры защиты от записи для книги.

```csharp
public class WriteProtection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | Получает и задает автора. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | Указывает, защищена ли эта рабочая книга от записи. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | Устанавливает защищённый пароль для изменения файла. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | Указывает, выбран ли параметр «Рекомендуется только чтение». |

## Методы

| Имя | Описание |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | Возвращает true, если указанный пароль совпадает с паролем защиты от записи, которым файл был защищён. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WriteProtectionDemo
    {
        public static void WriteProtectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к настройкам рабочей книги
            WorkbookSettings settings = workbook.Settings;

            // Получить доступ к настройкам защиты от записи
            WriteProtection writeProtection = settings.WriteProtection;

            // Установить автора защиты от записи
            writeProtection.Author = "John Doe";

            // Установить пароль для защиты от записи
            writeProtection.Password = "password123";

            // Установить рекомендованную опцию только для чтения
            writeProtection.RecommendReadOnly = true;

            // Проверить, защищена ли книга от записи
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // Проверить пароль
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // Сохраните книгу
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


