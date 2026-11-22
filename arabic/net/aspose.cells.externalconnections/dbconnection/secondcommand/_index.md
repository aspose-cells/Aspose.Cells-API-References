---
title: "DBConnection.SecondCommand"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DBConnection. تحدد سلسلة نصية للأمر الثاني تُحفظ عندما تكون حقول الصفحات المستندة إلى خادم PivotTable قيد الاستخدام. بالنسبة لاتصالات ODBC، يكون serverCommand عادةً استعلامًا أوسع من command حيث لا توجد جملة WHERE في الأول. بناءً على هذين الأمرين Command و ServerCommand يمكن ملء واجهة المستخدم للمعلمات ويمكن إنشاء استعلامات معلمة."
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/secondcommand/
---
## DBConnection.SecondCommand property

يحدد نص أمر ثانٍ يتم حفظه عندما تكون حقول الصفحات المستندة إلى الخادم في PivotTable قيد الاستخدام. في اتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة

```csharp
public override string SecondCommand { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء كائن DBConnection جديد بإضافته إلى المجموعة
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[0];
                
                // إعداد اتصال أساسي
                dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
                dbConnection.CommandType = OLEDBCommandType.SqlStatement;
                dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
                
                // تعيين وإظهار خاصية SecondCommand
                dbConnection.SecondCommand = "SELECT * FROM Customers";
                Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
                
                // تعديل SecondCommand لإظهار أنه قابل للكتابة
                dbConnection.SecondCommand = "SELECT * FROM Orders";
                Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
                
                // احفظ المصنف
                workbook.Save("SecondCommandDemo.xlsx");
                
                Console.WriteLine("SecondCommand demonstration completed successfully.");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


