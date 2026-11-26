---
title: "RevisionCellChange.IsNewFormatted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellChange. Указывает, является ли эта ячейка новоотформатированной"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/isnewformatted/
---
## RevisionCellChange.IsNewFormatted property

Указывает, отформатирована ли эта ячейка как новая.

```csharp
public bool IsNewFormatted { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsNewFormattedDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
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

            // Получите доступ к журналам ревизий
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Отобразить информацию о ревизии
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Продемонстрировать свойство IsNewFormatted
                        Console.WriteLine("\nFormatting Information:");
                        Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);
                        Console.WriteLine("IsNewFormatted: " + cellChange.IsNewFormatted);

                        if (cellChange.IsNewFormatted)
                        {
                            Console.WriteLine("The cell has new formatting applied in this revision.");
                            Console.WriteLine("New Font: " + cellChange.NewStyle.Font.Name);
                            Console.WriteLine("New Font Size: " + cellChange.NewStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + cellChange.NewStyle.Font.IsBold);
                        }
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellChangePropertyIsNewFormattedDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


