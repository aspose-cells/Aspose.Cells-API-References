---
title: "LightCellsDataHandler.StartSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LightCellsDataHandler. يبدأ في معالجة ورقة عمل"
type: docs
url: /ar/net/aspose.cells/lightcellsdatahandler/startsheet/
---
## LightCellsDataHandler.StartSheet method

يبدأ معالجة ورقة عمل.

```csharp
public bool StartSheet(Worksheet sheet)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ورقة | ورقة العمل | ورقة العمل لقراءة بيانات الخلايا. |

### قيمة الإرجاع

ما إذا كانت بيانات خلايا هذه الورقة تحتاج إلى المعالجة. false لتجاهل هذه الورقة.

### ملاحظات

سيتم استدعاؤها قبل قراءة بيانات خلايا ورقة العمل.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodStartSheetWithWorksheetDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                CustomLightCellsDataHandler handler = new CustomLightCellsDataHandler();
                bool result = handler.StartSheet(worksheet);

                Console.WriteLine($"StartSheet method returned: {result}");
                Console.WriteLine($"Worksheet name after StartSheet: {worksheet.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }

            workbook.Save("LightCellsDataHandlerStartSheetDemo.xlsx");
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            sheet.Name = "ModifiedByStartSheet";
            return true;
        }

        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


