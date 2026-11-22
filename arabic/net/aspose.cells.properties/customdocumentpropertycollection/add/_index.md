---
title: "CustomDocumentPropertyCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "CustomDocumentPropertyCollection method. ينشئ خاصية مستند مخصصة جديدة من نوع البيانات PropertyType.String"
type: docs
url: /ar/net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

إنشاء خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.String**.

```csharp
public DocumentProperty Add(string name, string value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية. |
| القيمة | String | قيمة الخاصية. |

### قيمة الإرجاع

كائن الخاصية الذي تم إنشاؤه حديثًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.CustomDocumentProperties.Add("startdate", "ToneyTest");
            
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["startdate"].Value);
                
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

إنشاء خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Number**.

```csharp
public DocumentProperty Add(string name, int value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية. |
| القيمة | Int32 | قيمة الخاصية. |

### قيمة الإرجاع

كائن الخاصية الذي تم إنشاؤه حديثًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet1");
            
            // إضافة خصائص مستند مخصصة
            workbook.CustomDocumentProperties.Add("textProperty", "Sample Text");
            workbook.CustomDocumentProperties.Add("numericProperty", 42);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحقق من الخصائص
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Text Property Value: " + loadedWorkbook.CustomDocumentProperties["textProperty"].Value);
            Console.WriteLine("Numeric Property Value: " + loadedWorkbook.CustomDocumentProperties["numericProperty"].Value);
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

إنشاء خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.DateTime**.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية. |
| القيمة | DateTime | قيمة الخاصية. |

### قيمة الإرجاع

كائن الخاصية الذي تم إنشاؤه حديثًا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Properties;

    public class CustomDocumentPropertyCollectionMethodAddWithStringDateTimeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // احصل على مجموعة خصائص المستند المخصصة
            CustomDocumentPropertyCollection customProps = workbook.Worksheets.CustomDocumentProperties;

            try
            {
                // أضف خاصية DateTime
                DateTime currentTime = DateTime.Now;
                DocumentProperty addedProp = customProps.Add("ReportGenerated", currentTime);

                // اعرض معلومات حول الخاصية المضافة
                Console.WriteLine($"Property Name : {addedProp.Name}");
                Console.WriteLine($"Property Type : {addedProp.Type}");
                Console.WriteLine($"Property Value: {addedProp.ToDateTime():O}");

                // احفظ المصنف (اختياري، يوضح أن الخاصية تستمر)
                workbook.Save("AddDateTimePropertyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding DateTime property: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

إنشاء خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Boolean**.

```csharp
public DocumentProperty Add(string name, bool value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية. |
| القيمة | منطقي | قيمة الخاصية. |

### قيمة الإرجاع

كائن الخاصية الذي تم إنشاؤه حديثًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // أضف خاصية مخصصة من نوع Boolean
            customProperties.Add("IsApproved", true);

            // اعرض الخاصية المضافة
            DocumentProperty property = customProperties["IsApproved"];
            Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");

            // احفظ المصنف
            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

إنشاء خاصية مستند مخصصة جديدة من نوع البيانات **PropertyType.Float**.

```csharp
public DocumentProperty Add(string name, double value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية. |
| القيمة | Double | قيمة الخاصية. |

### قيمة الإرجاع

كائن الخاصية الذي تم إنشاؤه حديثًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // أظهر طريقة Add مع معلمات String و Double
            customProperties.Add("Rating", 4.5);
            customProperties.Add("Score", 8.75);

            // الوصول إلى الخصائص المضافة وعرضها
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty scoreProperty = customProperties["Score"];

            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Score: {scoreProperty.ToDouble()}");

            workbook.Save("CustomDocumentPropertiesWithDoubleValues.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


