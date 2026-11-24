---
title: "Validation.Value1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validation-Eigenschaft. Stellt den ersten Wert dar, der mit der Datenvalidierung verknüpft ist."
type: docs
url: /de/net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Stellt den ersten Wert dar, der mit der Datenvalidierung verknüpft ist.

```csharp
public object Value1 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue1Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Validierung in Zelle A1.
            Validation validation = worksheet.Cells["A1"].GetValidation();
            validation.Type = ValidationType.List;
            
            // Setzen Sie die Value1-Eigenschaft mit einem String-Array.
            validation.Value1 = new object[] { "Option1", "Option2", "Option3" };

            // Abrufen und Anzeigen der Validierungswerte.
            object[] values = validation.Value1 as object[];
            Console.WriteLine("Validation values in A1:");
            foreach (object value in values)
            {
                Console.WriteLine(value.ToString());
            }

            // Erstellen Sie eine weitere Validierung in Zelle B1 mit unterschiedlichen Werten.
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Value1 = new object[] { "Yes", "No", "Maybe" };

            // Abrufen und Anzeigen der zweiten Validierungswerte.
            object[] values2 = validation2.Value1 as object[];
            Console.WriteLine("\nValidation values in B1:");
            foreach (object value in values2)
            {
                Console.WriteLine(value.ToString());
            }
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


