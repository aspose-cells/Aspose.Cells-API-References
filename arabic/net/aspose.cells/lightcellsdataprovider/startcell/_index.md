---
title: "LightCellsDataProvider.StartCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LightCellsDataProvider. تبدأ بحفظ بيانات خلية واحدة"
type: docs
url: /ar/net/aspose.cells/lightcellsdataprovider/startcell/
---
## LightCellsDataProvider.StartCell method

يبدأ بحفظ بيانات خلية واحدة.

```csharp
public void StartCell(Cell cell)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cell | Cell | كائن Cell للاستخدام في تنفيذ ملء البيانات. فهرس عموده هو القيمة المرجعة من آخر استدعاء لـ [`NextCell`](../nextcell/). إذا تم تهيئة الخلية في نموذج الخلايا الداخلي، سيتم استخدام كائن الخلية الموجود. وإلا سيتم استخدام كائن Cell مؤقت لتنفيذ ملء البيانات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartCellWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء خلية لاستخدامها كمعامل
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");
            
            // إنشاء موفر بيانات مخصص
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("StartCellWithCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with StartCell implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly int totalRows = 5;
            private readonly int totalCells = 3;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < totalRows ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < totalCells ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1}, Col {cell.Column + 1}");
            }

            public bool IsGatherString()
            {
                return false;
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


