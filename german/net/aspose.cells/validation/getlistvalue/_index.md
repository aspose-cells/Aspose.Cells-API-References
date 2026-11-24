---
title: "Validation.GetListValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungsmethode. Gibt den Wert für die Liste der Validierung für die angegebene Zelle zurück"
type: docs
url: /de/net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Liest den Wert für die Liste der Validierung für die angegebene Zelle.

```csharp
public object GetListValue(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

Der Wert, um die Liste dieser Validierung für die angegebene Zelle zu erzeugen. Wenn die Liste auf einen Bereich verweist, wird der zurückgegebene Wert ein [`ReferredArea`](../../referredarea/) Objekt sein; andernfalls kann der zurückgegebene Wert null, object[] oder ein einfaches Objekt sein.

### Hinweise

Nur für Validierungen, deren Typ List ist und die auf die angegebene Zelle angewendet wurden; andernfalls wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetListValueWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten für die Validierung hinzu.
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");

            // Erstelle eine Validierung für Zelle B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:A4";

            // Teste GetListValue mit verschiedenen Parametern
            Console.WriteLine("List values:");
            for (int i = 0; i < 4; i++)
            {
                object value = validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {value}");
            }

            // Ändere zu kommagetrennten Werten
            validation.Formula1 = "Red,Green,Blue";
            Console.WriteLine("\nComma-separated values:");
            for (int i = 0; i < 3; i++)
            {
                object[] values = (object[])validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
            }

            // Ändere zu einem einzelnen Wert
            validation.Formula1 = "SingleValue";
            Console.WriteLine("\nSingle value:");
            object singleValue = validation.GetListValue(0, 0);
            Console.WriteLine($"Value: {singleValue}");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


