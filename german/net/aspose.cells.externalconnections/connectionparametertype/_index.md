---
title: "Enum ConnectionParameterType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.ConnectionParameterType-Enum. Gibt den Parametertyp einer externen Verbindung an."
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparametertype/
---
## ConnectionParameterType enumeration

Gibt den Parametertyp der externen Verbindung an

```csharp
public enum ConnectionParameterType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Cell | `0` | Rufe den Parameterwert bei jeder Aktualisierung aus einer Zelle ab. |
| Prompt | `1` | Fordere den Benutzer bei jeder Aktualisierung zur Eingabe eines Parameterwerts auf. |
| Value | `2` | Verwende bei jeder Aktualisierung einen konstanten Wert für den Parameterwert. |

### Beispiele

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
                // Demonstriere das Erstellen und Verwenden von ConnectionParameterType-Enum-Werten.
                ConnectionParameterType cellParam = ConnectionParameterType.Cell;
                ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
                ConnectionParameterType valueParam = ConnectionParameterType.Value;

                // Die Enum-Werte anzeigen
                Console.WriteLine("Connection Parameter Types:");
                Console.WriteLine($"Cell: {cellParam}");
                Console.WriteLine($"Prompt: {promptParam}");
                Console.WriteLine($"Value: {valueParam}");

                // Demonstriere die Verwendung in einer switch-Anweisung.
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

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


