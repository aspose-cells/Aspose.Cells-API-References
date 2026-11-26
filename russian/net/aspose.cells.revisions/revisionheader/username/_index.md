---
title: "RevisionHeader.UserName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionHeader. Получает и задает имя пользователя, создающего ревизию"
type: docs
url: /ru/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Получает и задает имя пользователя, создающего ревизию.

```csharp
public string UserName { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Создайте экземпляр RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // Установите свойство UserName
                revisionHeader.UserName = "JohnDoe";

                // Отобразите текущее значение свойства UserName
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // Измените свойство UserName
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // Сохраните книгу, чтобы продемонстрировать использование свойства
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


