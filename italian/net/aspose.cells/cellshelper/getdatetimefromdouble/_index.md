---
title: "CellsHelper.GetDateTimeFromDouble"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di CellsHelper. Converte il valore double nel valore data/ora"
type: docs
url: /it/net/aspose.cells/cellshelper/getdatetimefromdouble/
---
## CellsHelper.GetDateTimeFromDouble method

Converte il valore double in valore data/ora.

```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| doubleValue | Double | Il valore double. |
| date1904 | Booleano | Sistema data 1904. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati per i parametri del metodo (Double, Boolean)
            double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
            bool date1904 = false; // Using 1900 date system

            try
            {
                // Chiama il metodo GetDateTimeFromDouble con i tipi di parametro specifici
                DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
                
                // Visualizza il risultato
                Console.WriteLine($"Converted DateTime: {result}");
                
                // Scrivi il risultato in una cella
                worksheet.Cells["A1"].PutValue("Original Double Value:");
                worksheet.Cells["B1"].PutValue(doubleValue);
                worksheet.Cells["A2"].PutValue("Converted DateTime:");
                worksheet.Cells["B2"].PutValue(result.ToString());
                
                Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


