---
title: "Класс RevisionCellChange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionCellChange. Представляет ревизию, изменяющую ячейки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncellchange/
---
## RevisionCellChange class

Представляет ревизию, изменяющую ячейки.

```csharp
public class RevisionCellChange : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | Получает имя ячейки. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | Получает индекс столбца ячейки. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | Указывает, отформатирована ли эта ячейка как новая. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | Указывает, отформатирована ли эта ячейка как старая. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | Получает старую формулу. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | Получает новый стиль ячейки. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | Получает новое значение ячейки. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | Получает старую формулу. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | Получает старый стиль ячейки. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | Получает старое значение ячейки. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | Получает индекс строки ячейки. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | Представляет тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionCellChangeDemo
    {
        public static void Run()
        {
            // Создать выходной каталог, если он не существует
            string outputDir = "output/";
            System.IO.Directory.CreateDirectory(outputDir);
            
            string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";

            // Создать начальную книгу и включить совместное использование
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Save(filePath, SaveFormat.Xlsx);

            // Повторно открыть книгу, чтобы внести отслеживаемые изменения
            Workbook workbook2 = new Workbook(filePath);
            Worksheet sheet = workbook2.Worksheets[0];
            
            // Первая ревизия: установить начальные значения
            sheet.Cells["A1"].PutValue("Initial Value");
            sheet.Cells["B2"].PutValue(100);
            workbook2.Save(filePath, SaveFormat.Xlsx);
            
            // Вторая ревизия: изменить значения
            sheet.Cells["A1"].PutValue("Updated Value");
            sheet.Cells["B2"].PutValue(200);
            workbook2.Save(filePath, SaveFormat.Xlsx);

            // Загрузить книгу, чтобы получить доступ к журналам ревизий
            Workbook workbook3 = new Workbook(filePath);
            
            // Обработать все журналы ревизий
            foreach (RevisionLog log in workbook3.Worksheets.RevisionLogs)
            {
                foreach (Revision rev in log.Revisions)
                {
                    if (rev.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange rcc = (RevisionCellChange)rev;
                        Console.WriteLine($"Revision Type: {rev.Type}");
                        Console.WriteLine($"Cell: {rcc.CellName} (Row: {rcc.Row}, Column: {rcc.Column})");
                        Console.WriteLine($"Old Value: {rcc.OldValue ?? "null"}");
                        Console.WriteLine($"New Value: {rcc.NewValue ?? "null"}");
                        Console.WriteLine("------------------------------------");
                    }
                }
            }
        }
    }
}
```

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


