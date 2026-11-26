---
title: "Перечисление CredentialsMethodType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExternalConnections.CredentialsMethodType. Указывает метод учётных данных, используемый для доступа к серверу"
type: docs
url: /ru/net/aspose.cells.externalconnections/credentialsmethodtype/
---
## CredentialsMethodType enumeration

Указывает метод учётных данных, используемый для доступа к серверу.

```csharp
public enum CredentialsMethodType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Integrated | `0` | Интегрированная аутентификация |
| None | `1` | Отсутствие учётных данных |
| Prompt | `2` | Запрос учётных данных |
| Stored | `3` | Сохранённые учётные данные |

### Примеры

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
                // Продемонстрировать все значения перечисления CredentialsMethodType
                Console.WriteLine("Available CredentialsMethodType values:");
                
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    Console.WriteLine($"{method} ({(int)method}) - {GetMethodDescription(method)}");
                }

                // Показать практическое использование с конкретным значением
                CredentialsMethodType selectedMethod = CredentialsMethodType.Integrated;
                Console.WriteLine($"\nSelected method: {selectedMethod}");
                
                // Продемонстрировать использование switch
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

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


