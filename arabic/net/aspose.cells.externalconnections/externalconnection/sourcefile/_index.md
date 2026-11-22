---
title: "ExternalConnection.SourceFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تُستخدم عندما يكون مصدر البيانات الخارجي ملفًا. عندما يفشل الاتصال بمثل هذا المصدر، يحاول تطبيق الجداول الاتصال مباشرةً بهذا الملف. قد يُعبّر عنه بصيغة URI أو بصيغة مسار ملف خاص بالنظام."
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/sourcefile/
---
## ExternalConnection.SourceFile property

يُستخدم عندما يكون مصدر البيانات الخارجي معتمدًا على ملف. عندما يفشل الاتصال بمثل هذا المصدر، تحاول تطبيق الجداول الإلكترونية الاتصال مباشرةً بهذا الملف. قد يُعبَّر عنه بصيغة URI أو بصيغة مسار ملف خاص بالنظام.

```csharp
public string SourceFile { get; set; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceFileDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("input.xlsx");
            ExternalConnectionCollection connections = workbook.DataConnections;

            foreach (ExternalConnection connection in connections)
            {
                if (!string.IsNullOrEmpty(connection.SourceFile))
                    connection.SourceFile = connection.SourceFile.Replace("C:\\", "D:\\");
            }

            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


