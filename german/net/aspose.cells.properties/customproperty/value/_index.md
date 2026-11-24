---
title: "CustomProperty.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomProperty Property. Gibt den Wert der benutzerdefinierten Property zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

Gibt den Wert der benutzerdefinierten Eigenschaft zurück oder setzt ihn.

```csharp
public string Value { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie eine benutzerdefinierte Eigenschaft mit einem langen Zeichenfolgenwert hinzu
            worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
            
            // Rufen Sie den Wert der benutzerdefinierten Eigenschaft ab und zeigen Sie ihn an
            string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Custom Property Value: " + propertyValue);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Laden Sie die Arbeitsmappe neu, um zu überprüfen, ob die Eigenschaft erhalten bleibt
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Überprüfen Sie, ob der Wert nach dem Laden derselbe ist
            string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
        }
    }
}
```

### Siehe auch

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


