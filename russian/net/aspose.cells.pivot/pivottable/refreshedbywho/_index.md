---
title: "PivotTable.RefreshedByWho"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает имя последнего пользователя, который обновил эту PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/refreshedbywho/
---
## PivotTable.RefreshedByWho property

Получает имя последнего пользователя, который обновил эту PivotTable.

```csharp
public string RefreshedByWho { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshedByWhoDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 8;

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pt = sheet.PivotTables[pivotIndex];
            
            // Добавить поля в сводную таблицу
            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Обновите сводную таблицу, чтобы установить свойство RefreshedByWho
            pt.RefreshData();
            pt.CalculateData();

            // Вывести информацию об обновлении
            Console.WriteLine("Pivot Table Refresh Information:");
            Console.WriteLine("Last Refresh Date: " + pt.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);
            
            // Сохраните и перезагрузите, чтобы продемонстрировать сохранность свойства
            string savePath = "PivotTableRefreshedByWhoDemo_Out.xlsx";
            wb.Save(savePath);
            
            // Перезагрузите книгу и проверьте свойство
            Workbook wb2 = new Workbook(savePath);
            PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
            Console.WriteLine("\nAfter Reload:");
            Console.WriteLine("Last Refresh Date: " + pt2.RefreshDate);
            Console.WriteLine("Refreshed By: " + pt2.RefreshedByWho);
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


