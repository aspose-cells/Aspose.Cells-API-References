---
title: "XlsSaveOptions.LightCellsDataProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XlsSaveOptions. موفر البيانات لحفظ المصنف في وضع LightCells"
type: docs
url: /ar/net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

مزود البيانات لحفظ المصنف في الوضع الخفيف.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // إنشاء خيارات حفظ XLS
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            
            // تعيين LightCellsDataProvider
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
            
            // حفظ المصنف بوضع LightCells
            workbook.Save("output.xls", saveOptions);
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
            return 0; // Only process first cell for demonstration
        }

        public int NextRow()
        {
            return 0; // Only process first row for demonstration
        }

        public void StartCell(Cell cell)
        {
            // تعيين قيمة سلسلة طويلة لتوضيح معالجة LightCells
            cell.PutValue(new string('X', 257));
        }

        public void StartRow(Row row)
        {
            // لا يلزم معالجة صفوف خاصة لهذا العرض التجريبي
        }

        public bool StartSheet(int sheetIndex)
        {
            // لا يلزم معالجة أوراق خاصة لهذا العرض التجريبي
            return false;
        }
    }
}
```

### انظر أيضًا

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


