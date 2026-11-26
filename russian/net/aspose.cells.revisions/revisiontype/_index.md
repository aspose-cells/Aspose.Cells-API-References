---
title: "Перечисление RevisionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Revisions.RevisionType перечисление. Представляет тип ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Представляет тип ревизии.

```csharp
public enum RevisionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| CustomView | `0` | Пользовательский вид. |
| DefinedName | `1` | Определённое имя. |
| ChangeCells | `2` | Изменение ячеек. |
| AutoFormat | `3` | Автоформат. |
| MergeConflict | `4` | Конфликт слияния. |
| Comment | `5` | Комментарий. |
| Format | `6` | Формат. |
| InsertSheet | `7` | Вставить лист. |
| MoveCells | `8` | Переместить ячейки. |
| Undo | `9` | Отменить. |
| QueryTable | `10` | Запрос к таблице. |
| InsertDelete | `11` | Вставка или удаление. |
| RenameSheet | `12` | Переименовать лист. |
| Unknown | `13` | Неизвестно. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Продемонстрировать использование разных значений перечисления RevisionType
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // Отобразить значения перечисления и их базовые целочисленные значения
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // Продемонстрировать проверку типов ревизий
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // Сохраните книгу
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


