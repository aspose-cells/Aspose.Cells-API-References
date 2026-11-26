---
title: "Класс ReferredArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.ReferredArea класс. Представляет ссылочную область по формуле"
type: docs
url: /ru/net/aspose.cells/referredarea/
---
## ReferredArea class

Представляет область, на которую ссылается формула.

```csharp
public class ReferredArea
```

## Свойства

| Имя | Описание |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | Конечный столбец области. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | Конечная строка области. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | Получить имя внешнего файла, если это внешняя ссылка. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | Указывает, является ли это областью. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | Указывает, содержит ли эта область все строки (полный столбец). |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | Указывает, содержит ли эта область все столбцы(полную строку). |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | Указывает, является ли это внешней ссылкой. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | Указывает, в каком листе находится эта ссылка. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | Имена всех листов, на которые ссылается этот экземпляр. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | Начальный столбец области. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | Начальная строка области. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | Получает значение ячейки с заданным смещением от верхнего левого угла этой области. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | Получает значение ячейки с заданным смещением от верхнего левого угла этой области. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | Получает значения ячеек в этой области. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | Получает значения ячеек в этой области. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | Возвращает адрес ссылки этой области. Обычно это адрес ссылки, который может использоваться в формуле, например "Sheet1!A1:C3". |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Настройте некоторые данные и формулу, которая ссылается на диапазон
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // Создайте формулу, которая ссылается на диапазон A1:B2
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // Получите ссылки на диапазоны из формулы
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // Получите первый ссылочный диапазон
                    ReferredArea referredArea = referredAreas[0];

                    // Отобразите базовые свойства ссылочного диапазона
                    Console.WriteLine($"Referred Area Details:");
                    Console.WriteLine($"- Is External Link: {referredArea.IsExternalLink}");
                    Console.WriteLine($"- Sheet Name: {referredArea.SheetName}");
                    Console.WriteLine($"- Start Row: {referredArea.StartRow}");
                    Console.WriteLine($"- Start Column: {referredArea.StartColumn}");
                    Console.WriteLine($"- End Row: {referredArea.EndRow}");
                    Console.WriteLine($"- End Column: {referredArea.EndColumn}");
                    Console.WriteLine($"- Is Area: {referredArea.IsArea}");
                    Console.WriteLine($"- Is Entire Row: {referredArea.IsEntireRow}");
                    Console.WriteLine($"- Is Entire Column: {referredArea.IsEntireColumn}");

                    // Получите значения из ссылочного диапазона
                    object values = referredArea.GetValues();
                    if (values is Array)
                    {
                        object[][] valueArray = (object[][])values;
                        Console.WriteLine("\nValues in the referred area:");
                        foreach (object[] row in valueArray)
                        {
                            foreach (object val in row)
                            {
                                Console.Write($"{val}\t");
                            }
                            Console.WriteLine();
                        }
                    }

                    // Получите конкретное значение из ссылочного диапазона
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // Отобразите адрес ссылки
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // Сохраните книгу
                workbook.Save("ReferredAreaDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReferredArea: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


