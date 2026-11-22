---
title: "Enum ProtectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ProtectionType enum. يمثل نوع حماية المصنف/ورقة العمل"
type: docs
url: /ar/net/aspose.cells/protectiontype/
---
## ProtectionType enumeration

يمثل نوع حماية المصنف/ورقة العمل.

```csharp
public enum ProtectionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| All | `0` | يمثل حماية الكل. |
| Contents | `1` | يمثل حماية المحتويات، يُستخدم في حماية ورقة العمل. |
| Objects | `2` | يمثل حماية الكائنات، يُستخدم في حماية ورقة العمل. |
| Scenarios | `3` | يمثل حماية السيناريوهات، يُستخدم في حماية ورقة العمل. |
| Structure | `4` | يمثل حماية البنية، يُستخدم في حماية المصنف. |
| Windows | `5` | يمثل حماية النافذة، يُستخدم في حماية المصنف. |
| None | `6` | يمثل عدم وجود حماية. فقط لخاصية القراءة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectionTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احمِ ورقة العمل بجميع أنواع الحماية
            worksheet.Protect(ProtectionType.All);
            
            // عرض كيفية الوصول إلى خصائص الحماية
            Console.WriteLine("Worksheet protection settings:");
            Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
            Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
            Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
            Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
            Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
            Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
            Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
            Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
            Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
            
            // إلغاء حماية ورقة العمل
            worksheet.Unprotect();
            
            // احمِ باستخدام أنواع حماية محددة
            worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
            Console.WriteLine("\nWorksheet protected with Contents and Objects only");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


