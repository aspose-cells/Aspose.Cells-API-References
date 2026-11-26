---
title: "RevisionCellChange.NewFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCellChange. Возвращает старую формулу"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/newformula/
---
## RevisionCellChange.NewFormula property

Получает старую формулу.

```csharp
public string NewFormula { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите начальную формулу в ячейку A1
            worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Измените формулу, чтобы создать ревизию
            worksheet.Cells["A1"].Formula = "=AVERAGE(B1:B3)";

            // Получите доступ к журналам ревизий
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // Отобразите информацию об изменении формулы
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Formula: " + cellChange.OldFormula);
                        Console.WriteLine("New Formula: " + cellChange.NewFormula);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Продемонстрируйте использование свойства NewFormula
                        if (!string.IsNullOrEmpty(cellChange.NewFormula))
                        {
                            Console.WriteLine("\nThe cell's new formula calculates: " + 
                                worksheet.Cells["A1"].StringValue);
                        }
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionCellChangePropertyNewFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


