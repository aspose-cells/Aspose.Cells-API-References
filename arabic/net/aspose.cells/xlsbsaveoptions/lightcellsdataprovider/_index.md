---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XlsbSaveOptions. موفر البيانات لحفظ المصنف في الوضع الخفيف"
type: docs
url: /ar/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

مزود البيانات لحفظ المصنف في الوضع الخفيف.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ بعض بيانات العينة
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // إنشاء خيارات حفظ XLSB
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // احفظ المصنف باستخدام LightCellsDataProvider
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // تحقق من البيانات المحفوظة
                stream.Seek(0, SeekOrigin.Begin);
                Workbook savedWorkbook = new Workbook(stream);
                Console.WriteLine("Workbook saved successfully with LightCellsDataProvider");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            // نفّذ منطق تكرار الخلايا هنا
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // نفّذ منطق تكرار الصفوف هنا
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // نفّذ منطق معالجة الخلايا هنا
        }

        public void StartRow(Row row)
        {
            // نفّذ منطق معالجة الصفوف هنا
        }

        public bool StartSheet(int sheetIndex)
        {
            // نفّذ منطق معالجة الورقة هنا
            return true; // Return true to process the sheet
        }
    }
}
```

### انظر أيضًا

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


