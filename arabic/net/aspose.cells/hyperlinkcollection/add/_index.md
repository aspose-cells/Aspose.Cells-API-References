---
title: "HyperlinkCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة HyperlinkCollection. تُضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | الصف الأول من نطاق الارتباط التشعبي. |
| firstColumn | Int32 | العمود الأول من نطاق الارتباط التشعبي. |
| totalRows | Int32 | عدد الصفوف في هذا النطاق التشعبي. |
| totalColumns | Int32 | عدد الأعمدة في هذا النطاق التشعبي. |
| address | String | عنوان الارتباط التشعبي. |

### قيمة الإرجاع

[`Hyperlink`](../../hyperlink/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة ارتباط تشعبي باستخدام إحداثيات الصف/العمود والأبعاد
            worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
            worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
            
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |
| totalRows | Int32 | عدد الصفوف في هذا النطاق التشعبي. |
| totalColumns | Int32 | عدد الأعمدة في هذا النطاق التشعبي. |
| address | String | عنوان الارتباط التشعبي. |

### قيمة الإرجاع

[`Hyperlink`](../../hyperlink/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // إضافة ارتباط تشعبي إلى الخلية A1 بالعنوان "www.aspose.com"
            hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            
            // عرض عنوان الارتباط التشعبي
            Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
            
            // تغيير نص العرض
            worksheet.Cells["A1"].PutValue("Click Here");
            Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
            
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startCellName | String | الخلية العلوية اليسرى للنطاق. |
| endCellName | String | الخلية السفلية اليمنى للنطاق. |
| address | String | عنوان الارتباط التشعبي. |
| textToDisplay | String | النص الذي سيتم عرضه للارتباط التشعبي المحدد. |
| screenTip | String | نص الـ screenTip للارتباط التشعبي المحدد. |

### قيمة الإرجاع

[`Hyperlink`](../../hyperlink/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // عرض طريقة Add مع معلمات (String, String, String, String, String)
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            workbook.Save("HyperlinkCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


