---
title: "LightCellsDataProvider.IsGatherString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LightCellsDataProvider. تتحقق مما إذا كانت قيمة النص الحالية للخلية تحتاج إلى جمعها في مجموعة عالمية"
type: docs
url: /ar/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

يتحقق مما إذا كانت قيمة السلسلة الحالية للخلية تحتاج إلى جمعها في مجموعة عالمية.

```csharp
public bool IsGatherString()
```

### قيمة الإرجاع

صحيح إذا كان يجب جمع قيمة النص في مجموعة عالمية للملف الناتج.

### ملاحظات

سيكون جمع قيم السلاسل مفيدًا فقط عندما يكون هناك العديد من قيم السلاسل المتكررة للخلايا التي يوفرها هذا التنفيذ. في هذه الحالة، سيوفر جمع السلاسل الكثير من الذاكرة وينتج ملفًا ناتجًا أصغر. إذا كان هناك العديد من قيم السلاسل للخلايا التي يوفرها LightCellsDataProvider لكن القليل منها متطابق، فإن جمع السلاسل سيستهلك المزيد من الذاكرة والوقت ولا يقدم أي فائدة للملف الناتج.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodIsGatherStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("IsGatherStringDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with IsGatherString implementation");
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
            private readonly object[,] data = new object[3, 2]
            {
                { "Product", "Price" },
                { "Laptop", 1200.50 },
                { "Phone", 899.99 }
            };

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 3 ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString()
            {
                // جمع السلاسل للصف العنوان فقط (rowIndex 0)
                return rowIndex == 0;
            }
        }
    }
}
```

### انظر أيضًا

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


