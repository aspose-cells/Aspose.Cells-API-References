---
title: "ExternalConnection.SecondCommand"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد سلسلة نصية للأمر الثاني تُحفظ عندما تكون حقول الصفحة المستندة إلى الخادم في PivotTable قيد الاستخدام. بالنسبة لاتصالات ODBC يكون serverCommand عادةً استعلامًا أوسع من command ولا توجد جملة WHERE في الأول. بناءً على هذين الأمرين command و ServerCommand يمكن ملء واجهة المستخدم للمعلمات ويمكن إنشاء استعلامات معلمة."
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

يحدد نص أمر ثانٍ يتم حفظه عندما تكون حقول الصفحات المستندة إلى الخادم في PivotTable قيد الاستخدام. في اتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة

```csharp
public virtual string SecondCommand { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // اعرض القيمة الحالية لـ SecondCommand (عملية قراءة)
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // عيّن قيمة جديدة لـ SecondCommand (نظرًا لأنه قابل للقراءة والكتابة)
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // امسح SecondCommand لتوضيح تعيين سلسلة فارغة
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("SecondCommandDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


