---
title: "LineFormat.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LineFormat. Determina se questa istanza ha lo stesso valore di un altro oggetto LineFormat specificato"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Determina se questa istanza ha lo stesso valore di un altro oggetto [`LineFormat`](../) specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | L'oggetto [`LineFormat`](../) da confrontare con questa istanza. |

### Valore di ritorno

true se il valore del parametro obj è lo stesso del valore di questa istanza; altrimenti, false. Se obj è null, questo metodo restituisce false.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma linea al foglio di lavoro
            worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
            
            // Ottieni il formato della linea della prima forma
            LineFormat lineFmt1 = worksheet.Shapes[0].Line;
            LineFormat lineFmt2 = worksheet.Shapes[0].Line;
            
            // Confronta i formati della linea usando il metodo Equals
            if (lineFmt1.Equals((object)lineFmt2))
            {
                Console.WriteLine("The line formats are equal.");
            }
            else
            {
                Console.WriteLine("The line formats are not equal.");
            }
        }
    }
}
```

### Vedi anche

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


