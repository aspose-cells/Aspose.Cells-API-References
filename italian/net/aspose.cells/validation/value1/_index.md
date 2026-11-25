---
title: "Validation.Value1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Validation. Rappresenta il primo valore associato alla convalida dei dati"
type: docs
url: /it/net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Rappresenta il primo valore associato alla convalida dei dati.

```csharp
public object Value1 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue1Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una convalida nella cella A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            validation.Type = ValidationType.List;
            
            // Imposta la proprietà Value1 con un array di stringhe
            validation.Value1 = new object[] { "Option1", "Option2", "Option3" };

            // Ottieni e visualizza i valori della convalida
            object[] values = validation.Value1 as object[];
            Console.WriteLine("Validation values in A1:");
            foreach (object value in values)
            {
                Console.WriteLine(value.ToString());
            }

            // Crea un'altra convalida nella cella B1 con valori diversi
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Value1 = new object[] { "Yes", "No", "Maybe" };

            // Ottieni e visualizza i valori della seconda convalida
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

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


