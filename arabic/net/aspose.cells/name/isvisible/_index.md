---
title: "Name.IsVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Name. تشير إلى ما إذا كان الاسم مرئيًا"
type: docs
url: /ar/net/aspose.cells/name/isvisible/
---
## Name.IsVisible property

يشير إلى ما إذا كان الاسم مرئيًا.

```csharp
public bool IsVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق مسمى مرئي
            int visibleIndex = workbook.Worksheets.Names.Add("VisibleRange");
            Name visibleName = workbook.Worksheets.Names[visibleIndex];
            visibleName.RefersTo = "=Sheet1!$A$1:$B$2";
            visibleName.IsVisible = true;
            
            // إنشاء نطاق مسمى مخفي
            int hiddenIndex = workbook.Worksheets.Names.Add("HiddenRange");
            Name hiddenName = workbook.Worksheets.Names[hiddenIndex];
            hiddenName.RefersTo = "=Sheet1!$C$1:$D$2";
            hiddenName.IsVisible = false;
            
            // عرض خاصية IsVisible
            Console.WriteLine("VisibleRange IsVisible: " + visibleName.IsVisible);
            Console.WriteLine("HiddenRange IsVisible: " + hiddenName.IsVisible);
            
            // احفظ المصنف
            workbook.Save("NameVisibilityDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


