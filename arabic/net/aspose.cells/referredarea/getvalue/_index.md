---
title: "ReferredArea.GetValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ReferredArea. تحصل على قيمة الخلية مع الإزاحة المحددة من الزاوية العليا اليسرى لهذا النطاق"
type: docs
url: /ar/net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | إزاحة الصف من الصف الأول لهذا النطاق |
| colOffset | Int32 | إزاحة العمود من الصف الأول لهذا النطاق |

### قيمة الإرجاع

"#REF!" إذا كان هذا النطاق غير صالح؛ "#N/A" إذا كانت الإزاحة المحددة خارج هذا النطاق؛ وإلا إرجاع قيمة الخلية في الموضع المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = "=A1";
            
            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                object value = referredAreas[0].GetValue(0, 0);
                Console.WriteLine("Value at (0,0): " + value);
            }
        }
    }
}
```

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | إزاحة الصف من الصف الأول لهذا النطاق |
| colOffset | Int32 | إزاحة العمود من الصف الأول لهذا النطاق |
| calculateFormulas | منطقي | ما إذا كان يجب حسابه بشكل متكرر إذا كان المرجع المحدد صيغة |

### قيمة الإرجاع

"#REF!" إذا كان هذا النطاق غير صالح؛ "#N/A" إذا كانت الإزاحة المحددة خارج هذا النطاق؛ وإلا إرجاع قيمة الخلية في الموضع المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(100);
            sheet.Cells["B1"].PutValue(200);

            workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names["TestRange"];
            name.RefersTo = "=Sheet1!$A$1:$B$1";

            ReferredArea ra = name.GetReferredAreas(true)[0];
            object result = ra.GetValue(0, 0, true);

            Console.WriteLine("Obtained value: " + result);
        }
    }
}
```

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


