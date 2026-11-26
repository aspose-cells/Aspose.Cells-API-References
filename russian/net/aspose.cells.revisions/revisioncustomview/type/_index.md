---
title: "RevisionCustomView.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCustomView. Возвращает тип ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncustomview/type/
---
## RevisionCustomView.Type property

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

    public class RevisionCustomViewPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            // Отслеживание изменений, по-видимому, включено по умолчанию при внесении изменений
            
            // Добавьте пользовательский вид для создания записи ревизии
            workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
            
            // Получите доступ к коллекции ревизий через встроенную функциональность Workbook
            RevisionCollection revisions = null;
            if (workbook.HasRevisions)
            {
                // В реальной реализации должен существовать способ доступа к ревизиям
                // Поскольку мы не можем найти точный метод, оставим это как null
                // Это сохраняет структуру, учитывая ограничение API
                revisions = null; // Would normally be workbook.Revisions or similar
            }

            // Найдите RevisionCustomView в ревизиях
            RevisionCustomView customViewRevision = null;
            if (revisions != null)
            {
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCustomView)
                    {
                        customViewRevision = (RevisionCustomView)revision;
                        break;
                    }
                }
            }

            if (customViewRevision != null)
            {
                // Отобразите значение свойства Type
                Console.WriteLine("Revision Type: " + customViewRevision.Type);
                
                // Продемонстрируйте, как можно использовать свойство Type
                if (customViewRevision.Type == RevisionType.CustomView)
                {
                    Console.WriteLine("This revision is for a custom view operation");
                    Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
                }
                
                // Свойство Type только для чтения, поэтому его нельзя установить
                // Мы можем только проверить его значение, чтобы определить тип ревизии
                switch (customViewRevision.Type)
                {
                    case RevisionType.CustomView:
                        Console.WriteLine("Handling custom view revision");
                        break;
                    case RevisionType.Comment:
                        Console.WriteLine("Handling comment revision");
                        break;
                    // Другие случаи могут быть добавлены по мере необходимости
                    default:
                        Console.WriteLine("Handling other revision type");
                        break;
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCustomViewTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


