---
title: "ExternalConnection.Parameters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. يحصل على ConnectionParameterCollection لاستعلام ODBC أو ويب"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/parameters/
---
## ExternalConnection.Parameters property

يحصل على [`ConnectionParameterCollection`](../../connectionparametercollection/) لاستعلام ODBC أو ويب.

```csharp
public ConnectionParameterCollection Parameters { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyParametersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // عرض معلومات مجموعة Parameters
                ConnectionParameterCollection parameters = connection.Parameters;
                Console.WriteLine($"Number of parameters: {parameters.Count}");
                
                // عرض معلومات كل معلمة إذا كانت متاحة
                foreach (ConnectionParameter param in parameters)
                {
                    Console.WriteLine($"Parameter name: {param.Name}");
                    Console.WriteLine($"Parameter type: {param.Type}");
                    Console.WriteLine($"Parameter prompt: {param.Prompt}");
                    Console.WriteLine("----------------------");
                }
                
                // احفظ المصنف
                workbook.Save("ParametersDemo.xlsx");
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

* class [ConnectionParameterCollection](../../connectionparametercollection/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


