---
title: "Workbook.RemoveMacro"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تُزيل VBA/ماكرو من هذا جدول البيانات"
type: docs
url: /ar/net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

يزيل VBA/ماكرو من هذه الورقة الإلكترونية.

```csharp
public void RemoveMacro()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveMacroDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل من ملف مُمكّن للماكرو موجود
            Workbook workbook = new Workbook("example.xlsm");

            // إزالة الماكرو من دفتر العمل
            workbook.RemoveMacro();
            
            // حفظ كدفتر عمل خالٍ من الماكرو
            string noMacroPath = "NoMacro.xlsx";
            workbook.Save(noMacroPath, SaveFormat.Xlsx);

            Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


