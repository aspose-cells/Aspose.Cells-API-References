---
title: "Validation.GetValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Validation. Ottieni il valore della convalida nella cella specifica"
type: docs
url: /it/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

Ottieni il valore della convalida sulla cella specifica.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |
| isValue1 | Booleano | Indica se si sta ottenendo il primo valore. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e convalida
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // Crea una convalida per la cella B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // Ottieni il valore usando il metodo GetValue con parametri riga, colonna e conversione da numerico a data
            object value = validation.GetValue(0, 1, false);
            
            // Restituisci il risultato
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


