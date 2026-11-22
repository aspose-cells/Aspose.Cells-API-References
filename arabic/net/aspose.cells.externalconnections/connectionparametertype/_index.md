---
title: "تعداد ConnectionParameterType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ExternalConnections.ConnectionParameterType. يحدد نوع المعامل للاتصال الخارجي"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparametertype/
---
## ConnectionParameterType enumeration

يحدد نوع المعلمة للاتصال الخارجي

```csharp
public enum ConnectionParameterType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Cell | `0` | احصل على قيمة المعامل من خلية في كل تحديث. |
| Prompt | `1` | اطلب من المستخدم قيمة المعامل في كل تحديث. |
| Value | `2` | استخدم قيمة ثابتة في كل تحديث لقيمة المعامل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterTypeDemo
    {
        public static void Run()
        {
            try
            {
                // عرض إنشاء واستخدام قيم تعداد ConnectionParameterType
                ConnectionParameterType cellParam = ConnectionParameterType.Cell;
                ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
                ConnectionParameterType valueParam = ConnectionParameterType.Value;

                // عرض قيم التعداد
                Console.WriteLine("Connection Parameter Types:");
                Console.WriteLine($"Cell: {cellParam}");
                Console.WriteLine($"Prompt: {promptParam}");
                Console.WriteLine($"Value: {valueParam}");

                // إظهار الاستخدام في جملة switch
                ConnectionParameterType testParam = ConnectionParameterType.Prompt;
                switch (testParam)
                {
                    case ConnectionParameterType.Cell:
                        Console.WriteLine("Parameter will get value from a cell");
                        break;
                    case ConnectionParameterType.Prompt:
                        Console.WriteLine("Parameter will prompt user for value");
                        break;
                    case ConnectionParameterType.Value:
                        Console.WriteLine("Parameter will use constant value");
                        break;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating ConnectionParameterType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


