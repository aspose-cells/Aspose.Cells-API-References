---
title: "ReferredArea.SheetNames"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReferredArea. Имена всех листов, на которые ссылается этот экземпляр."
type: docs
url: /ru/net/aspose.cells/referredarea/sheetnames/
---
## ReferredArea.SheetNames property

Имена всех листов, на которые ссылается этот экземпляр.

```csharp
public string[] SheetNames { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertySheetNamesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы создать ссылку на формулу.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Вычислите формулы, чтобы получить ссылки.
            workbook.CalculateFormula();

            // Получите ссылочную область из формулы в ячейке A3.
            ReferredArea referredArea = worksheet.Cells["A3"].GetPrecedents()[0];

            // Отобразите свойство SheetNames.
            Console.WriteLine("SheetNames referenced by the formula:");
            if (referredArea.SheetNames != null)
            {
                foreach (string sheetName in referredArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Добавьте еще один лист и создайте межлистовую ссылку.
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=Sheet1!A3");

            // Снова вычислите формулы.
            workbook.CalculateFormula();

            // Получить ссылочную область из формулы, ссылающейся на другой лист
            ReferredArea crossSheetArea = sheet2.Cells["B1"].GetPrecedents()[0];

            // Отобразить имена листов для кросс-листовой ссылки
            Console.WriteLine("\nSheetNames referenced by cross-sheet formula:");
            if (crossSheetArea.SheetNames != null)
            {
                foreach (string sheetName in crossSheetArea.SheetNames)
                {
                    Console.WriteLine(sheetName);
                }
            }

            // Сохраните книгу
            workbook.Save("ReferredAreaSheetNamesDemo.xlsx");
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


