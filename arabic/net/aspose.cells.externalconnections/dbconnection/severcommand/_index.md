---
title: "DBConnection.SeverCommand"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DBConnection. تحدد سلسلة نصية للأمر الثاني تُحفظ عندما تكون حقول الصفحات المستندة إلى خادم PivotTable قيد الاستخدام. بالنسبة لاتصالات ODBC، يكون serverCommand عادةً استعلامًا أوسع من command حيث لا توجد جملة WHERE في الأول. بناءً على هذين الأمرين Command و ServerCommand يمكن ملء واجهة المستخدم للمعلمات ويمكن إنشاء استعلامات معلمة."
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/severcommand/
---
## DBConnection.SeverCommand property

يحدد نص أمر ثانٍ يتم حفظه عندما تكون حقول الصفحات المستندة إلى الخادم في PivotTable قيد الاستخدام. في اتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). استنادًا إلى هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة

```csharp
[Obsolete("Use ExternalConnection.SecondCommand property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SeverCommand { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.SecondCommand. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class DBConnectionPropertySeverCommandDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("input.xlsx");
            ExternalConnectionCollection connections = workbook.DataConnections;

            foreach (ExternalConnection connection in connections)
            {
                if (connection is DBConnection dbConn)
                {
                    dbConn.Name = dbConn.Name.Replace("c:\\", "d:\\");
                    dbConn.SourceFile = dbConn.SourceFile.Replace("c:\\", "d:\\");
                    dbConn.ConnectionInfo = dbConn.ConnectionInfo.Replace("c:\\", "d:\\").Replace("C:\\", "d:\\");
                    dbConn.Command = dbConn.Command.Replace("c:\\", "d:\\");
                    
                    if (!string.IsNullOrEmpty(dbConn.SeverCommand))
                        dbConn.SeverCommand = dbConn.SeverCommand.Replace("c:\\", "d:\\");
                }
            }

            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


