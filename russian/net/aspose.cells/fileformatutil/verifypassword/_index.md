---
title: "FileFormatUtil.VerifyPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FileFormatUtil. Обнаруживает и возвращает информацию о формате Excel, хранящегося в потоке"
type: docs
url: /ru/net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

Определяет и возвращает информацию о формате Excel, хранящегося в потоке.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream |  |
| пароль | String | Пароль для зашифрованных файлов ooxml. |

### Возвращаемое значение

Возвращает, корректен ли пароль.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodVerifyPasswordWithStreamStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            string correctPassword = "test";
            string wrongPassword = "1234";

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, correctPassword);
                Console.WriteLine($"Password '{correctPassword}' is valid: {isValid}");
            }

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, wrongPassword);
                Console.WriteLine($"Password '{wrongPassword}' is valid: {isValid}");
            }
        }
    }
}
```

### См. также

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


