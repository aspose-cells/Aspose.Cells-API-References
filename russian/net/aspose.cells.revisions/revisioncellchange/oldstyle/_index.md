---
title: "RevisionCellChange.OldStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellChange. Возвращает старый стиль ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/oldstyle/
---
## RevisionCellChange.OldStyle property

Получает старый стиль ячейки.

```csharp
public Style OldStyle { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить начальный стиль для ячейки A1
            Cell cell = worksheet.Cells["A1"];
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            initialStyle.Font.Color = System.Drawing.Color.Black;
            cell.SetStyle(initialStyle);
            cell.PutValue("Initial Value");

            // Изменить стиль ячейки, чтобы создать ревизию
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.Color = System.Drawing.Color.Red;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);
            cell.PutValue("Modified Value");

            // Получите доступ к журналам ревизий
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // Отобразить информацию об изменении стиля
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Style Font: " + cellChange.OldStyle.Font.Name);
                        Console.WriteLine("Old Style Size: " + cellChange.OldStyle.Font.Size);
                        Console.WriteLine("Old Style Color: " + cellChange.OldStyle.Font.Color);
                        Console.WriteLine("New Style Font: " + cellChange.NewStyle.Font.Name);
                        Console.WriteLine("New Style Size: " + cellChange.NewStyle.Font.Size);
                        Console.WriteLine("New Style Color: " + cellChange.NewStyle.Font.Color);

                        // Продемонстрировать использование свойства OldStyle
                        if (cellChange.OldStyle.Font.Name == "Arial")
                        {
                            Console.WriteLine("\nThe cell originally had Arial font");
                        }
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellChangePropertyOldStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


