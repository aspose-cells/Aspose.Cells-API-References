---
title: "Enum ReConnectionMethodType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExternalConnections.ReConnectionMethodType. Указывает, что приложение таблиц должно делать при сбое соединения"
type: docs
url: /ru/net/aspose.cells.externalconnections/reconnectionmethodtype/
---
## ReConnectionMethodType enumeration

Указывает, что должно делать приложение таблиц, когда соединение не удаётся.

```csharp
public enum ReConnectionMethodType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Required | `1` | При обновлении используйте существующую информацию о соединении, и если она окажется недействительной, получите обновлённую информацию о соединении, если она доступна во внешнем файле соединения. |
| Always | `2` | При каждом обновлении получайте обновлённую информацию о соединении из внешнего файла соединения, если он доступен, и используйте её вместо существующей информации о соединении. В этом случае обновление данных завершится неудачей, если внешний файл соединения недоступен. |
| Never | `3` | Никогда не получать обновлённую информацию о соединении из внешнего файла соединения, даже если он доступен и даже если существующая информация о соединении недействительна |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassReConnectionMethodTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Продемонстрировать создание и использование значений перечисления ReConnectionMethodType
                ReConnectionMethodType method1 = ReConnectionMethodType.Required;
                ReConnectionMethodType method2 = ReConnectionMethodType.Always;
                ReConnectionMethodType method3 = ReConnectionMethodType.Never;

                Console.WriteLine("ReConnectionMethodType values:");
                Console.WriteLine($"Required: {(int)method1}");
                Console.WriteLine($"Always: {(int)method2}");
                Console.WriteLine($"Never: {(int)method3}");

                // Показать использование в операторе switch
                Console.WriteLine("\nDemonstrating switch usage:");
                TestConnectionMethod(method1);
                TestConnectionMethod(method2);
                TestConnectionMethod(method3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReConnectionMethodType: {ex.Message}");
            }
        }

        private static void TestConnectionMethod(ReConnectionMethodType method)
        {
            switch (method)
            {
                case ReConnectionMethodType.Required:
                    Console.WriteLine("Using Required reconnection method");
                    break;
                case ReConnectionMethodType.Always:
                    Console.WriteLine("Using Always reconnection method");
                    break;
                case ReConnectionMethodType.Never:
                    Console.WriteLine("Using Never reconnection method");
                    break;
                default:
                    Console.WriteLine("Unknown reconnection method");
                    break;
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


