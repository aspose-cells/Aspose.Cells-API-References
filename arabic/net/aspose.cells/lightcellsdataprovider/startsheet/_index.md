---
title: "LightCellsDataProvider.StartSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LightCellsDataProvider. يبدأ بحفظ ورقة عمل"
type: docs
url: /ar/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

يبدأ بحفظ ورقة عمل.

```csharp
public bool StartSheet(int sheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | Int32 | فهرس الورقة الحالية التي سيتم حفظها. |

### قيمة الإرجاع

true إذا كان هذا الموفر سيزود البيانات للورقة المحددة؛ false إذا كان يجب على الورقة المحددة استخدام نموذج البيانات العادي (Cells).

### ملاحظات

سيتم استدعاؤه في بداية حفظ ورقة عمل أثناء حفظ دفتر العمل. إذا كان الموفر يحتاج إلى الإشارة إلى

```csharp
sheetIndex
```

لاحقًا في طريقة startRow(Row) أو startCell(Cell)، أي إذا كانت العملية تحتاج إلى معرفة أي ورقة عمل يتم معالجتها، يجب على التنفيذ الاحتفاظ بـ

```csharp
sheetIndex
```

القيمة هنا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartSheetWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                workbook.Worksheets.Clear(); // Start with clean worksheet
                
                // إنشاء موفر بيانات مخصص وحفظه باستخدام وضع الخلايا الخفيفة
                var saveOptions = new OoxmlSaveOptions
                {
                    LightCellsDataProvider = new CustomLightCellsDataProvider()
                };

                Console.WriteLine("Starting workbook save with LightCellsDataProvider...");
                workbook.Save("StartSheetDemoOutput.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully. Check StartSheetDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private bool sheetProcessed = false;

            // يتم استدعاؤه عند بدء معالجة ورقة العمل
            public bool StartSheet(int sheetIndex)
            {
                Console.WriteLine($"Processing sheet index: {sheetIndex}");
                // معالجة الورقة الأولى فقط (الفهرس 0)
                if (sheetIndex == 0)
                {
                    sheetProcessed = true;
                    return true;
                }
                return false;
            }

            public int NextRow()
            {
                if (sheetProcessed)
                {
                    sheetProcessed = false;
                    return 0; // Process first row (index 0)
                }
                return -1; // Stop processing after first row
            }

            public void StartRow(Row row)
            {
                row.Height = 20;
            }

            public int NextCell()
            {
                return 0; // Process first cell (index 0)
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue("Data from LightCellsDataProvider");
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

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


