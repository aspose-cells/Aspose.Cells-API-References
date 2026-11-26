---
title: "RevisionCellChange.NewStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellChange. Возвращает новый стиль ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/newstyle/
---
## RevisionCellChange.NewStyle property

Получает новый стиль ячейки.

```csharp
public Style NewStyle { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            // Прямой метод StartTrackingRevisions недоступен — ревизии отслеживаются автоматически
            Worksheet worksheet = workbook.Worksheets[0];

            // Измените ячейку, чтобы создать ревизию
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 10;
            cell.SetStyle(originalStyle);

            // Измените ячейку, чтобы создать ревизию
            cell.PutValue("New Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            // Прямой метод StopTrackingRevisions недоступен

            // Получите доступ к журналу ревизий через RevisionLogs вместо Revisions
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Отобразите информацию о ревизии изменения ячейки
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Получите доступ к свойству NewStyle
                        Style revisionNewStyle = cellChange.NewStyle;
                        Console.WriteLine("\nNew Style Properties:");
                        Console.WriteLine("Font Name: " + revisionNewStyle.Font.Name);
                        Console.WriteLine("Font Size: " + revisionNewStyle.Font.Size);
                        Console.WriteLine("Is Bold: " + revisionNewStyle.Font.IsBold);
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellChangePropertyNewStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


