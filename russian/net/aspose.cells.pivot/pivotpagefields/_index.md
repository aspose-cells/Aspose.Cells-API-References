---
title: "Класс PivotPageFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotPageFields. Представляет элементы страниц сводной таблицы, если источник данных сводной таблицы — диапазоны консолидации. Может содержать не более 4 элементов."
type: docs
url: /ru/net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

Представляет элементы страниц сводной таблицы, если источник данных сводной таблицы — диапазоны консолидации. Может содержать не более 4 элементов.

```csharp
public class PivotPageFields
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PivotPageFields](pivotpagefields/)() | Представляет элементы полей страниц сводной таблицы. |

## Свойства

| Имя | Описание |
| --- | --- |
| [PageFieldCount](../../aspose.cells.pivot/pivotpagefields/pagefieldcount/) { get; } | Получает количество полей страниц. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddIdentify](../../aspose.cells.pivot/pivotpagefields/addidentify/)(int, int[]) | Устанавливает, какую метку элемента в каждом поле страницы использовать для идентификации диапазона данных. Длина pageItemIndex должна быть равна PageFieldCount, поэтому сначала добавьте поле страницы. |
| [AddPageField](../../aspose.cells.pivot/pivotpagefields/addpagefield/)(string[]) | Добавляет поле страницы. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotPageFieldsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Sheet1";
            FillData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            FillData(sheet2);

            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;

            string[] src = { "=Sheet1!A1:C8", "=Sheet2!A1:C8" };
            PivotPageFields pageFields = new PivotPageFields();

            pageFields.AddPageField(new string[] { "item1", "item2" });
            pageFields.AddPageField(new string[] { "item3", "item4" });

            pageFields.AddIdentify(0, new int[] { 0, 1 });
            pageFields.AddIdentify(1, new int[] { 1, -1 });

            pivotTables.Add(src, false, pageFields, "E3", "PivotTable1");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }

        private static void FillData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Value");
            cells["C1"].PutValue("Date");

            for (int i = 1; i < 8; i++)
            {
                cells[$"A{i+1}"].PutValue($"Item{i}");
                cells[$"B{i+1}"].PutValue(i * 100);
                cells[$"C{i+1}"].PutValue(System.DateTime.Now.AddDays(i).ToString("yyyy-MM-dd"));
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


