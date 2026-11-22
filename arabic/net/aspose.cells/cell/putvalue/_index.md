---
title: "Cell.PutValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تضع قيمة منطقية في الخلية"
type: docs
url: /ar/net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

يضع قيمة منطقية في الخلية.

```csharp
public void PutValue(bool boolValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| boolValue | منطقي |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ضع قيمة منطقية في الخلية B3 (الصف 2، العمود 2)
            cells[2, 2].PutValue(true);

            // تحقق من أن القيمة تم تعيينها بشكل صحيح
            Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

يضع قيمة عددية صحيحة في الخلية.

```csharp
public void PutValue(int intValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| intValue | Int32 | قيمة الإدخال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // استخدام PutValue مع معلمات Int32
            cells[0, 0].PutValue(10);
            cells[1, 0].PutValue(20);
            cells[2, 0].PutValue(30);
            
            // احسب مجموع القيم
            cells[3, 0].Formula = "=SUM(A1:A3)";
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

يضع قيمة مزدوجة في الخلية.

```csharp
public void PutValue(double doubleValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| doubleValue | Double | قيمة الإدخال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // ضع قيم مزدوجة باستخدام طريقة PutValue
            cells[0, 0].PutValue("Item");
            cells[0, 1].PutValue("Price");
            cells[1, 0].PutValue("Apple");
            cells[1, 1].PutValue(0.69);
            cells[2, 0].PutValue("Banana");
            cells[2, 1].PutValue(0.49);
            cells[3, 0].PutValue("Orange");
            cells[3, 1].PutValue(0.29);

            // احفظ المصنف
            workbook.Save("PutValueWithDoubleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

يضع قيمة في الخلية، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الأرقام للخلية.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | String | قيمة الإدخال |
| isConverted | منطقي | صحيح: تم تحويله إلى نوع بيانات آخر إذا كان مناسبًا. |
| setStyle | منطقي | صحيح: تعيين تنسيق الرقم إلى نمط الخلية عند التحويل إلى نوع بيانات آخر |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على الخلية B3
            Cell cell = worksheet.Cells["B3"];
            
            // تعيين التحقق من صحة البيانات للعمر (يجب أن يكون رقمًا موجبًا)
            Validation validation = cell.GetValidation();
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "0";
            
            // ضع قيمة مع التحويل وفحص التحقق
            cell.PutValue("-60", true, false);
            
            // احسب الصيغ (على الرغم من أنها غير ضرورية في هذه الحالة البسيطة)
            workbook.CalculateFormula();
            
            // تحقق مما إذا كانت القيمة صالحة
            bool isValid = cell.GetValidationValue();
            Console.WriteLine("Is value valid? " + isValid);
            
            // احفظ دفتر العمل
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

يضع قيمة سلسلة في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | String | قيمة الإدخال |
| isConverted | منطقي | صحيح: تم تحويله إلى نوع بيانات آخر إذا كان مناسبًا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // عرض PutValue مع معلمات النص والقيمة المنطقية
            cells["B2"].PutValue("123", true);  // String value with conversion flag
            cells["C2"].PutValue("456", false); // String value without conversion
            
            // تحقق من القيم
            Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
            Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string

            workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

يضع قيمة سلسلة في الخلية.

```csharp
public void PutValue(string stringValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | String | قيمة الإدخال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // استخدام PutValue مع معلمات السلسلة
            cells[0, 0].PutValue("Product");
            cells[0, 1].PutValue("Category");
            cells[0, 2].PutValue("Price");
            
            cells[1, 0].PutValue("Laptop");
            cells[1, 1].PutValue("Electronics");
            cells[1, 2].PutValue(999.99);
            
            cells[2, 0].PutValue("Desk Chair");
            cells[2, 1].PutValue("Furniture");
            cells[2, 2].PutValue(199.50);
            
            // احفظ المصنف
            workbook.Save("PutValueStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

يضع قيمة تاريخ/وقت في الخلية.

```csharp
public void PutValue(DateTime dateTime)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dateTime | DateTime | قيمة الإدخال |

### ملاحظات

تعيين قيمة DateTime لخلية لا يعني أن الخلية سيتم تنسيقها كوقت وتاريخ تلقائيًا. تم الحفاظ على قيمة DateTime كقيمة رقمية في نموذج البيانات لكل من MS Excel و Aspose.Cells. ما إذا كانت القيمة الرقمية ستُعامل كقيمة رقمية نفسها أو كوقت وتاريخ يعتمد على تنسيق الرقم المطبق على هذه الخلية. إذا لم يتم تنسيق هذه الخلية كوقت وتاريخ، فستُعرض كقيمة رقمية رغم أن ما أدخلته هو DateTime.

### أمثلة

يوضح هذا المثال كيفية تعيين قيمة DateTime لخلية وجعلها تُعرض كوقت وتاريخ.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//إدراج وقت وتاريخ في خلية
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

يضع قيمة كائن في الخلية.

```csharp
public void PutValue(object objectValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| objectValue | Object | قيمة الإدخال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue مع كائن DateTime
            DateTime dt = new DateTime(2008, 2, 2);
            cells[0, 0].PutValue((object)dt);
            
            // PutValue مع كائن سلسلة
            cells[1, 0].PutValue((object)"Hello World");
            
            // PutValue مع كائن رقمي
            cells[2, 0].PutValue((object)123.45);
            
            // احفظ المصنف
            workbook.Save("PutValueWithObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


