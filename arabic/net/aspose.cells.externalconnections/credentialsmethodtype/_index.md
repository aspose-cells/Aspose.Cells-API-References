---
title: "Enum CredentialsMethodType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ExternalConnections.CredentialsMethodType enum. يحدد طريقة الاعتمادات المستخدمة للوصول إلى الخادم"
type: docs
url: /ar/net/aspose.cells.externalconnections/credentialsmethodtype/
---
## CredentialsMethodType enumeration

يحدد طريقة الاعتماد المستخدمة للوصول إلى الخادم.

```csharp
public enum CredentialsMethodType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Integrated | `0` | المصادقة المتكاملة |
| None | `1` | بدون اعتمادات |
| Prompt | `2` | طلب الاعتمادات |
| Stored | `3` | الاعتمادات المخزنة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            try
            {
                // عرض جميع قيم enum الخاصة بـ CredentialsMethodType
                Console.WriteLine("Available CredentialsMethodType values:");
                
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    Console.WriteLine($"{method} ({(int)method}) - {GetMethodDescription(method)}");
                }

                // عرض الاستخدام العملي بقيمة محددة
                CredentialsMethodType selectedMethod = CredentialsMethodType.Integrated;
                Console.WriteLine($"\nSelected method: {selectedMethod}");
                
                // توضيح استخدام switch
                switch (selectedMethod)
                {
                    case CredentialsMethodType.Integrated:
                        Console.WriteLine("Using integrated authentication");
                        break;
                    case CredentialsMethodType.None:
                        Console.WriteLine("No credentials will be used");
                        break;
                    case CredentialsMethodType.Prompt:
                        Console.WriteLine("User will be prompted for credentials");
                        break;
                    case CredentialsMethodType.Stored:
                        Console.WriteLine("Using stored credentials");
                        break;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating CredentialsMethodType: {ex.Message}");
            }
        }

        private static string GetMethodDescription(CredentialsMethodType method)
        {
            return method switch
            {
                CredentialsMethodType.Integrated => "Integrated Authentication",
                CredentialsMethodType.None => "No Credentials",
                CredentialsMethodType.Prompt => "Prompt Credentials",
                CredentialsMethodType.Stored => "Stored Credentials",
                _ => "Unknown method"
            };
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


