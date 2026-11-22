---
title: "MarkdownSaveOptions.LightCellsDataProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MarkdownSaveOptions. موفر البيانات لتوفير بيانات الخلايا لحفظ المصنف في الوضع الخفيف"
type: docs
url: /ar/net/aspose.cells/markdownsaveoptions/lightcellsdataprovider/
---
## MarkdownSaveOptions.LightCellsDataProvider property

موفر البيانات لتوفير بيانات الخلايا لحفظ المصنف في وضع خفيف.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections.Generic;

    public class MarkdownSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ بعض بيانات العينة
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Item " + (i + 1);
                worksheet.Cells[i, 1].Value = i + 1;
            }

            // إنشاء LightCellsDataProvider مخصص
            var dataProvider = new CustomLightCellsDataProvider();

            // إنشاء MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            
            // عرض القيمة الحالية (يجب أن تكون null في البداية)
            Console.WriteLine("Current LightCellsDataProvider value: " + (saveOptions.LightCellsDataProvider == null ? "null" : "set"));

            // تعيين موفر البيانات المخصص
            saveOptions.LightCellsDataProvider = dataProvider;

            // حفظ باستخدام موفر البيانات المخصص
            workbook.Save("LightCellsDataProviderDemo.md", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private List<string> items = new List<string> { "Apple", "Banana", "Cherry", "Date", "Elderberry" };
        private List<double> values = new List<double> { 1.99, 0.99, 2.99, 3.49, 4.99 };
        private int currentRow = -1;

        public bool StartSheet(int sheetIndex)
        {
            // معالجة الورقة الأولى فقط
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            return currentRow < items.Count ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // تعيين ارتفاع الصف إذا لزم الأمر
            row.Height = 15;
        }

        public int NextCell()
        {
            if (currentRow == -1)
            {
                // صف الرأس
                return currentRow < 2 ? currentRow + 1 : -1;
            }
            else
            {
                return currentRow < 2 ? currentRow + 1 : -1;
            }
        }

        public void StartCell(Cell cell)
        {
            if (currentRow == -1)
            {
                // رأس الصفحة
                if (cell.Column == 0)
                    cell.Value = "Product";
                else if (cell.Column == 1)
                    cell.Value = "Price";
            }
            else
            {
                // البيانات
                if (cell.Column == 0)
                    cell.Value = items[currentRow];
                else if (cell.Column == 1)
                    cell.Value = values[currentRow];
            }
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### انظر أيضًا

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


