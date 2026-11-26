---
title: "UnionRange.RefersTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Получает диапазоны, к которым относится"
type: docs
url: /ru/net/aspose.cells/unionrange/refersto/
---
## UnionRange.RefersTo property

Получает значение свойства RefersTo диапазона.

```csharp
public string RefersTo { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми данными
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Создать именованный диапазон
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("B2:B3");
            namedRange.Name = "ProductPrices";

            // Создайте объединённый диапазон, который включает наш именованный диапазон
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B3").UnionRanges(new Aspose.Cells.Range[] { namedRange });

            // Отобразите свойство RefersTo объединённого диапазона
            Console.WriteLine("UnionRange RefersTo: " + unionRange.RefersTo);

            // Создайте другой диапазон и отобразите его RefersTo
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("C1:D3");
            Console.WriteLine("Single Range RefersTo: " + singleRange.RefersTo);

            // Продемонстрируйте использование RefersTo для определения состава диапазона
            Console.WriteLine("Does union range contain named range? " + 
                unionRange.RefersTo.Contains("ProductPrices"));

            // Покажите, как RefersTo меняется при изменении диапазонов
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C3");
            UnionRange modifiedUnion = newRange.UnionRanges(new Aspose.Cells.Range[] { namedRange });
            Console.WriteLine("Modified UnionRange RefersTo: " + modifiedUnion.RefersTo);

            // Сохраните книгу
            workbook.Save("UnionRangeRefersToDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


