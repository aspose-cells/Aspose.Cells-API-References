---
title: "Validation.GetValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Methode. Gibt den Wert der Validierung in der angegebenen Zelle zurück"
type: docs
url: /de/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

Liest den Wert der Validierung für die spezifische Zelle.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |
| isValue1 | Boolean | Gibt an, ob der erste Wert abgerufen wird. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und Validierung hinzufügen
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // Erstelle eine Validierung für Zelle B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // Wert mit der GetValue-Methode unter Angabe von Zeile, Spalte und den Parametern zum Konvertieren numerischer Werte in ein Datum abrufen
            object value = validation.GetValue(0, 1, false);
            
            // Gib das Ergebnis aus
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


