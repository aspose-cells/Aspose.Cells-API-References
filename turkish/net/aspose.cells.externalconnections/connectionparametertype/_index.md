---
title: "Enum ConnectionParameterType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.ConnectionParameterType enum. Harici bağlantının parametre tipini belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparametertype/
---
## ConnectionParameterType enumeration

Harici bağlantının parametre tipini belirtir

```csharp
public enum ConnectionParameterType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Cell | `0` | Her yenilemede parametre değerini bir hücreden al. |
| Prompt | `1` | Her yenilemede kullanıcıdan bir parametre değeri isteme. |
| Value | `2` | Parametre değeri için her yenilemede sabit bir değer kullan. |

### Örnekler

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
                // ConnectionParameterType enum değerlerini oluşturma ve kullanma örneği
                ConnectionParameterType cellParam = ConnectionParameterType.Cell;
                ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
                ConnectionParameterType valueParam = ConnectionParameterType.Value;

                // Enum değerlerini görüntüle
                Console.WriteLine("Connection Parameter Types:");
                Console.WriteLine($"Cell: {cellParam}");
                Console.WriteLine($"Prompt: {promptParam}");
                Console.WriteLine($"Value: {valueParam}");

                // Bir switch ifadesinde kullanımını göster
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


