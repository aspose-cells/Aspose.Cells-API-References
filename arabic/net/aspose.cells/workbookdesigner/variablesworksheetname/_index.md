---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookDesigner. تحصل وتعيّن اسم ورقة العمل التي تحتوي على علامة المتغيرات الذكية"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

يحصل ويضبط اسم ورقة العمل التي تحتوي على متغيرات smart marker.

```csharp
public string VariablesWorksheetName { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyVariablesWorksheetNameDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();

                // إضافة ورقة عمل باسم "Variables" لتوضيح الخاصية
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // إنشاء مثيل WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // عرض قيمة VariablesWorksheetName الحالية
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // تعيين قيمة جديدة لـ VariablesWorksheetName
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // إضافة ورقة عمل أخرى مع علامات ذكية
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // معالجة العلامات الذكية
                designer.Process();

                // احفظ المصنف
                workbook.Save("VariablesWorksheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with VariablesWorksheetName set.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


