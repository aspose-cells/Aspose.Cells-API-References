---
title: "Cell.GetDisplayStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة الخلية. تحصل على نمط العرض لهذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

يحصل على نمط العرض لهذه الخلية.

```csharp
public Style GetDisplayStyle()
```

### قيمة الإرجاع

نمط العرض لهذه الخلية

### ملاحظات

نفس الشيء عند استخدام SideBorders لـ `GetDisplayStyle`. أي أن هذه الطريقة ستتحقق وتضبط حدود الأعلى/الأسفل/اليسار/اليمين لهذه الخلية وفقًا للنمط ([`GetStyle`](../getstyle/)) للخلايا المجاورة، ولكن لا تتحقق من الخلايا المدمجة، ولا تتحقق من نمط العرض للخلايا المجاورة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين النمط للخلية A1
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.FromArgb(157, 195, 230);
            worksheet.Cells["A1"].SetStyle(style1);
            
            // تعيين النمط للخلية A23
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Red;
            worksheet.Cells["A23"].SetStyle(style2);
            
            // احصل على الأنماط وعرضها
            Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
            Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
            
            Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
            Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(bool) {#getdisplaystyle_2}

يحصل على نمط العرض لهذه الخلية.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| includeMergedBorders | منطقي | يشير إلى ما إذا كان يتم فحص حدود الخلايا المدمجة. |

### قيمة الإرجاع

نمط العرض لهذه الخلية

### ملاحظات

إذا كانت العلامة المحددة خاطئة، فستكون النتيجة مماثلة لـ `GetDisplayStyle`. وإلا فستكون مماثلة لاستخدام SideBorders&#x7C;DynamicStyleBorders لـ `GetDisplayStyle`.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية B2 وتعيين بعض خصائص النمط
            Cell cell = worksheet.Cells["B2"];
            Style cellStyle = cell.GetStyle();
            cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            cell.SetStyle(cellStyle);
            
            // احصل على نمط العرض مع التنسيق (معامل true)
            Style displayStyle = cell.GetDisplayStyle(true);
            
            // إخراج نمط خط الحد الأيمن
            Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

يحصل على نمط العرض لهذه الخلية.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| adjacentBorders | BorderType | يشير إلى الحدود التي يجب فحصها وتعديلها وفقًا لحدود الخلايا المجاورة. |

### قيمة الإرجاع

نمط العرض لهذه الخلية

### ملاحظات

إذا كانت هذه الخلية متأثرة أيضًا بإعدادات أخرى مثل التنسيق الشرطي، كائنات القوائم، إلخ، فقد يكون نمط العرض مختلفًا عن [`GetStyle`](../getstyle/). بالنسبة للعلامات التي تضبط الحدود وفقًا للخلايا المجاورة، فإن TopBorder/BottomBorder/LeftBorder/RightBorder تشير إلى ما إذا كان سيتم فحص ودمج حدود الأسفل/الأعلى/اليمين/اليسار للخلايا اليسرى/اليمنى/العليا/السفلى المجاورة لهذه الخلية. لأغراض الأداء والتوافق، تُستخدم بعض القيم العددية (enums) للدلالة على عمليات خاصة: Horizontal/Vertical تشير إلى ما إذا كان سيتم فحص ودمج حد الأسفل/اليمين للخلايا المدمجة مع هذه الخلية. Diagonal (أي أن كلًا من DiagonalUpBorder و DiagonalDownBorder تم تعيينهما) تشير إلى فحص ودمج الحدود من نمط عرض الخلايا المجاورة. يرجى ملاحظة أن فحص حدود/أنماط الخلايا المجاورة، خاصةً أنماط العرض، عملية تستغرق وقتًا. إذا لم يكن هناك حاجة للحصول على الحدود للنمط المرجع، فإن استخدام None لتعطيل عملية الخلايا المجاورة سيعطي أداءً أفضل. عند الحصول على حدود الخلايا المجاورة من الأنماط المعرفة على تلك الخلايا فقط (دون تعيين Diagonal)، قد يكون الأداء أيضًا أفضل لأن فحص نمط عرض خلية واحدة يستغرق وقتًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBorderTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // تعيين بيانات عينة
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // إنشاء تنسيق شرطي
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // احصل على نمط العرض بأنواع حدود مختلفة
            for (int i = 0; i < 10; i++)
            {
                Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
                Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);

                Console.WriteLine($"Cell {i + 1}:");
                Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
                Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


