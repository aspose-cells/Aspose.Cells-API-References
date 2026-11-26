---
title: "RevisionInsertSheet.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionInsertSheet. Возвращает тип правки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertsheet/type/
---
## RevisionInsertSheet.Type property

Получает тип ревизии.

```csharp
public override RevisionType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            
            // Включите отслеживание правок (симулировано, так как StartTrackingRevisions недоступен)
            bool trackRevisions = true;

            // Добавьте новый лист для создания записи правки
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Смоделируйте получение правок (поскольку свойство Revisions недоступно)
            if (trackRevisions && workbook.HasRevisions)
            {
                // В реальном сценарии мы бы получили доступ к правкам здесь
                // Это предполагает, что мы получили правку откуда-то (например, из workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                if (insertSheetRevision != null)
                {
                    // Отобразите свойство Type
                    Console.WriteLine("Revision Type: " + insertSheetRevision.Type);

                    // Продемонстрируйте использование свойства Type, доступного только для чтения
                    if (insertSheetRevision.Type == RevisionType.InsertSheet)
                    {
                        Console.WriteLine("This revision represents a sheet insertion operation");
                        
                        // Покажите дополнительную информацию о вставленном листе
                        Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
                        Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
                    }

                    // Проверьте против других типов правок
                    if (insertSheetRevision.Type != RevisionType.Unknown)
                    {
                        Console.WriteLine("This is a known revision type");
                    }
                }

                // Сохраните книгу
                workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No revisions found or revision tracking not enabled");
            }
        }
    }
}
```

### См. также

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


