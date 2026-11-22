---
title: "BuiltInDocumentPropertyCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تُعيد كائن DocumentProperty باسم الخاصية"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

تُرجع كائن [`DocumentProperty`](../../documentproperty/) باسم الخاصية.

```csharp
public override DocumentProperty this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم الخاصية غير حساس لحالة الأحرف المراد استرجاعه. |

### ملاحظات

أسماء السلاسل للخصائص تتطابق مع أسماء الخصائص المكتوبة المتاحة من [`BuiltInDocumentPropertyCollection`](../).

إذا طلبت خاصية غير موجودة في المستند، لكن اسم الخاصية يُعترف به كاسم مدمج صالح، يتم إنشاء [`DocumentProperty`](../../documentproperty/) جديد، يُضاف إلى المجموعة ويُعاد. تُعطى الخاصية التي تم إنشاؤها حديثًا قيمةً افتراضية (سلسلة فارغة، صفر، خاطئ أو DateTime.MinValue حسب نوع الخاصية المدمجة).

إذا طلبت خاصية غير موجودة في المستند ولم يُعترف بالاسم كاسم مدمج، يتم إرجاع قيمة فارغة (null).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // عيّن خاصية مستند مدمجة باستخدام الطريقة المناسبة
            workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
            
            // الوصول إلى قيمة الخاصية وطباعةها
            Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // حمّل دفتر العمل المحفوظ وتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


