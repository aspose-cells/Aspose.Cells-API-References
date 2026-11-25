---
title: "Validation.GetListValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Validation. Ottieni il valore per l'elenco della convalida per la cella specificata"
type: docs
url: /it/net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Ottieni il valore per l'elenco della convalida per la cella specificata.

```csharp
public object GetListValue(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |

### Valore di ritorno

Il valore per generare l'elenco di questa convalida per la cella specificata. Se l'elenco fa riferimento a un intervallo, il valore restituito sarà un oggetto [`ReferredArea`](../../referredarea/); altrimenti il valore restituito può essere null, object[] o un semplice oggetto.

### Osservazioni

Solo per le convalide il cui tipo è List e che sono state applicate alla cella indicata; altrimenti verrà restituito null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetListValueWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la convalida
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");

            // Crea una convalida per la cella B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:A4";

            // Testa GetListValue con parametri diversi
            Console.WriteLine("List values:");
            for (int i = 0; i < 4; i++)
            {
                object value = validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {value}");
            }

            // Modifica in valori separati da virgola
            validation.Formula1 = "Red,Green,Blue";
            Console.WriteLine("\nComma-separated values:");
            for (int i = 0; i < 3; i++)
            {
                object[] values = (object[])validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
            }

            // Modifica a valore singolo
            validation.Formula1 = "SingleValue";
            Console.WriteLine("\nSingle value:");
            object singleValue = validation.GetListValue(0, 0);
            Console.WriteLine($"Value: {singleValue}");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


