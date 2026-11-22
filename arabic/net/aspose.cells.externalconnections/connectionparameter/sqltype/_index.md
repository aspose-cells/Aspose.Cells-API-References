---
title: "ConnectionParameter.SqlType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConnectionParameter. نوع بيانات SQL للمعامل. صالح فقط لمصادر ODBC"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparameter/sqltype/
---
## ConnectionParameter.SqlType property

نوع بيانات SQL للمعامل. صالح فقط لمصادر ODBC.

```csharp
public SqlDataType SqlType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertySqlTypeDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                
                // إنشاء معامل اتصال (محاكى لأن معلمات المُنشئ غير معروفة)
                ConnectionParameter parameter = null;
                
                // في سيناريو حقيقي، ستقوم بإنشاء المعامل بشكل صحيح
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // للتوضيح، سنظهر كيف سيتم استخدام SqlType إذا كان لدينا معامل
                if (parameter != null)
                {
                    // احصل على قيمة SqlType الحالية واعرضها
                    Console.WriteLine("Current SqlType: " + parameter.SqlType);
                    
                    // قم بتعيين قيمة SqlType جديدة (لأن الخاصية قابلة للقراءة والكتابة)
                    parameter.SqlType = SqlDataType.SqlInteger;
                    Console.WriteLine("Updated SqlType: " + parameter.SqlType);
                }
                else
                {
                    // عرض بديل عندما لا نستطيع إنشاء المعامل
                    workbook.Worksheets[0].Cells["A1"].Value = "SqlType property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterSqlTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [SqlDataType](../../sqldatatype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


