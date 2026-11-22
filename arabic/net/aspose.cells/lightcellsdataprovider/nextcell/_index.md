---
title: "LightCellsDataProvider.NextCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LightCellsDataProvider. تحصل على الخلية التالية لحفظها"
type: docs
url: /ar/net/aspose.cells/lightcellsdataprovider/nextcell/
---
## LightCellsDataProvider.NextCell method

يحصل على الخلية التالية التي سيتم حفظها.

```csharp
public int NextCell()
```

### قيمة الإرجاع

فهرس العمود للخلية التالية لحفظها. -1 يعني أنه تم الوصول إلى نهاية بيانات الصف الحالي ولا توجد خلية أخرى من الصف الحالي لحفظها.

### ملاحظات

سيتم استدعاؤه في بداية حفظ خلية واحدة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var provider = new DemoLightCellsDataProvider();
            XlsSaveOptions saveOptions = new XlsSaveOptions { LightCellsDataProvider = provider };

            try
            {
                workbook.Save("NextCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class DemoLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly object[,] data = new object[2, 2]
            {
                { "Column1", "Column2" },
                { 100, 200 }
            };

            public bool StartSheet(int sheetIndex) => sheetIndex == 0;

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 2 ? 1 : 0;
            }

            public void StartRow(Row row) { }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? 1 : 0;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString() => false;
        }
    }
}
```

### انظر أيضًا

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


