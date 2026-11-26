---
title: "RevisionCellChange.IsOldFormatted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "RevisionCellChange property. Указывает, является ли эта ячейка староотформатированной"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/isoldformatted/
---
## RevisionCellChange.IsOldFormatted property

Указывает, отформатирована ли эта ячейка как старая.

```csharp
public bool IsOldFormatted { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsOldFormattedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить начальное значение ячейки и стиль
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            cell.SetStyle(initialStyle);

            // Изменить значение и стиль ячейки, чтобы создать ревизию
            cell.PutValue("Updated Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Calibri";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            try
            {
                // Получите доступ к журналам ревизий
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Отобразить значение свойства IsOldFormatted
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);

                            // Показать дополнительный контекст о ревизии
                            if (cellChange.IsOldFormatted)
                            {
                                Console.WriteLine("The cell had formatting before this revision.");
                                Console.WriteLine("Old Font: " + cellChange.OldStyle.Font.Name);
                                Console.WriteLine("Old Font Size: " + cellChange.OldStyle.Font.Size);
                            }
                            else
                            {
                                Console.WriteLine("The cell did not have formatting before this revision.");
                            }
                        }
                    }
                }

                // Сохранить книгу с ревизиями
                workbook.Save("IsOldFormattedDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved as IsOldFormattedDemo.xlsx");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


