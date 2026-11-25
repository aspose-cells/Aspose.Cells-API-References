---
title: "UnionRange.PutValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnionRange. Inserisce un valore nell'intervallo; se appropriato il valore verrà convertito in un altro tipo di dato e il formato numerico delle celle verrà ripristinato"
type: docs
url: /it/net/aspose.cells/unionrange/putvalue/
---
## UnionRange.PutValue method

Inserisce un valore nell'intervallo; se opportuno il valore sarà convertito in un altro tipo di dati e il formato numerico della cella verrà ripristinato.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | String | Valore di input |
| isConverted | Booleano | True: convertito in un altro tipo di dato se appropriato. |
| setStyle | Booleano | True: imposta il formato numerico nello stile della cella quando si converte in un altro tipo di dato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo di unione che copre le celle A1 a B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            
            try
            {
                // Chiama PutValue con i parametri: (String, Boolean, Boolean)
                unionRange.PutValue("Sample Value", true, true);
                
                Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
                
                // Visualizza le informazioni dell'intervallo per mostrare l'effetto
                Console.WriteLine($"Range address: {unionRange.RefersTo}");
                Console.WriteLine($"Value set in range: {unionRange.Value}");
                
                // Applica la formattazione per rendere visibile l'effetto
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.HorizontalAlignment = TextAlignmentType.Center;
                unionRange.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PutValue method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


