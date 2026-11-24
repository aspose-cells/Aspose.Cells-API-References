---
title: "Klasse ConnectionParameter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.ConnectionParameter Klasse. Gibt Eigenschaften zu allen Parametern an, die mit externen Datenverbindungen verwendet werden. Parameter sind gültig für ODBC- und Webabfragen."
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparameter/
---
## ConnectionParameter class

Gibt Eigenschaften zu allen Parametern an, die mit externen Datenverbindungen verwendet werden. Parameter sind für ODBC‑ und Web‑Abfragen gültig.

```csharp
public class ConnectionParameter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | Zellreferenz, die angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. Wird nur verwendet, wenn parameterType Zelle ist. |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | Der Name des Parameters. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | Eingabeaufforderungszeichenfolge für den Parameter. Wird dem Tabellenbenutzer zusammen mit einer Eingabe‑UI präsentiert, um den Parameterwert vor dem Aktualisieren der externen Daten zu erfassen. Wird nur verwendet, wenn parameterType = prompt. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | Flag, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert liefert, ändert. Wenn wahr, werden die externen Daten bei jeder Änderung mit dem neuen Parameterwert aktualisiert. Wenn falsch, werden die externen Daten nur aktualisiert, wenn der Benutzer dies anfordert oder ein anderes Ereignis die Aktualisierung auslöst (z. B. beim Öffnen der Arbeitsmappe). |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | SQL-Datentyp des Parameters. Nur gültig für ODBC-Quellen. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | Typ des verwendeten Parameters. Wenn parameterType=Wert, wird der Wert aus Boolean, Double, Integer oder String verwendet. In diesem Fall wird erwartet, dass nur einer von {Boolean, Double, Integer oder String} angegeben wird. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | Nicht‑ganzzahliger numerischer Wert, Ganzzahlwert, Zeichenkettenwert oder Boolescher Wert, der als Abfrageparameter verwendet wird. Wird nur verwendet, wenn parameterType Wert ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle einen Verbindungsparameter mittels Reflexion, da der Konstruktor nicht öffentlich ist.
                ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
                
                // Grundlegende Eigenschaften festlegen
                parameter.Name = "CustomerID";
                parameter.Type = ConnectionParameterType.Value;
                parameter.Value = "CUST1001";
                parameter.RefreshOnChange = true;
                parameter.Prompt = "Enter Customer ID:";
                
                // Parameterinformationen anzeigen
                Console.WriteLine($"Created parameter: {parameter.Name}");
                Console.WriteLine($"Type: {parameter.Type}");
                Console.WriteLine($"Value: {parameter.Value}");
                Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
                Console.WriteLine($"Prompt: {parameter.Prompt}");
                
                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionParameterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


