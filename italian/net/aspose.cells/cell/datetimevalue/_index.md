---
title: "Cell.DateTimeValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottiene il valore DateTime contenuto nella cella"
type: docs
url: /it/net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Restituisce il valore DateTime contenuto nella cella.

```csharp
public DateTime DateTimeValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDateTimeValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta un valore DateTime nella cella A1
            DateTime testDate = new DateTime(2023, 12, 25);
            cells["A1"].PutValue(testDate);

            // Formatta la cella per visualizzare la data
            Style style = cells["A1"].GetStyle();
            style.Custom = "yyyy-MM-dd";
            cells["A1"].SetStyle(style);

            // Recupera e verifica il DateTimeValue
            DateTime retrievedDate = cells["A1"].DateTimeValue;
            Console.WriteLine("Original DateTime: " + testDate.ToString("yyyy-MM-dd"));
            Console.WriteLine("Retrieved DateTime: " + retrievedDate.ToString("yyyy-MM-dd"));

            // Imposta un altro valore DateTime nella cella B1
            DateTime anotherDate = new DateTime(2024, 1, 1);
            cells["B1"].PutValue(anotherDate);

            // Visualizza il DateTimeValue da B1
            Console.WriteLine("B1 DateTime: " + cells["B1"].DateTimeValue.ToString("yyyy-MM-dd"));
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


