---
title: "الفئة ConnectionParameter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ExternalConnections.ConnectionParameter. تحدد الخصائص المتعلقة بأي معلمات تُستخدم مع اتصالات البيانات الخارجية. المعلمات صالحة لـ ODBC واستعلامات الويب."
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparameter/
---
## ConnectionParameter class

يحدد الخصائص المتعلقة بأي معلمات تُستخدم مع اتصالات البيانات الخارجية. المعلمات صالحة لاستعلامات ODBC والويب.

```csharp
public class ConnectionParameter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | مرجع الخلية الذي يشير إلى قيمة الخلية التي يجب استخدامها لمعلمة الاستعلام. يُستخدم فقط عندما يكون parameterType هو cell. |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | اسم المعلمة. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | سلسلة المطالبة للمعلمة. تُعرض على مستخدم الجدول مع واجهة إدخال لجمع قيمة المعلمة قبل تحديث البيانات الخارجية. تُستخدم فقط عندما يكون parameterType = prompt. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | علامة تشير إلى ما إذا كان يجب تحديث الاستعلام تلقائيًا عندما يتغير محتوى الخلية التي توفر قيمة المعامل. إذا كان true، يتم تحديث البيانات الخارجية باستخدام قيمة المعامل الجديدة في كل مرة يحدث فيها تغيير. إذا كان false، يتم تحديث البيانات الخارجية فقط عند طلب المستخدم أو عندما يُ triggers حدث آخر (مثل فتح المصنف). |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | نوع بيانات SQL للمعامل. صالح فقط لمصادر ODBC. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | نوع المعامل المستخدم. إذا كان parameterType=value، فسيتم استخدام القيمة من boolean أو double أو integer أو string. في هذه الحالة، من المتوقع تحديد أحد {boolean, double, integer, or string} فقط. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | قيمة عددية غير صحيحة، قيمة صحيحة، قيمة نصية أو قيمة منطقية لاستخدامها كمعامل للاستعلام. تُستخدم فقط عندما يكون parameterType هو value. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء معامل اتصال باستخدام الانعكاس لأن المُنشئ غير عام.
                ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
                
                // تعيين الخصائص الأساسية
                parameter.Name = "CustomerID";
                parameter.Type = ConnectionParameterType.Value;
                parameter.Value = "CUST1001";
                parameter.RefreshOnChange = true;
                parameter.Prompt = "Enter Customer ID:";
                
                // عرض معلومات المعامل.
                Console.WriteLine($"Created parameter: {parameter.Name}");
                Console.WriteLine($"Type: {parameter.Type}");
                Console.WriteLine($"Value: {parameter.Value}");
                Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
                Console.WriteLine($"Prompt: {parameter.Prompt}");
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


