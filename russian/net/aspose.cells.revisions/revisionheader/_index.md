---
title: "Класс RevisionHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Revisions.RevisionHeader класс. Представляет список конкретных изменений, произошедших в этой рабочей книге"
type: docs
url: /ru/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Представляет список конкретных изменений, которые произошли в этой рабочей книге.

```csharp
public class RevisionHeader
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RevisionHeader](revisionheader/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Получает и задает дату и время, когда этот набор ревизий был сохранён. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Получает и задает имя пользователя, создающего ревизию. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте экземпляр класса RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // Установите необходимые свойства
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // Продемонстрируйте базовую функциональность
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // Сохраните книгу
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


