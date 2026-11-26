---
title: "RevisionHeader.SavedTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionHeader. Получает и задает дату и время, когда этот набор ревизий был сохранён"
type: docs
url: /ru/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

Получает и задает дату и время, когда этот набор ревизий был сохранён.

```csharp
public DateTime SavedTime { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertySavedTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте экземпляр RevisionHeader
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // Установите свойство SavedTime
                revisionHeader.SavedTime = DateTime.Now;
                
                // Получите и отобразите значение SavedTime
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // Измените свойство SavedTime
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // Сохраните книгу, чтобы продемонстрировать использование свойства
                workbook.Save("SavedTimeDemo.xlsx");
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


