---
title: "Style.Custom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Rappresenta la stringa di formato numerico personalizzato di questo oggetto stile. Se il formato numerico personalizzato non è impostato, ad esempio verrà restituito il formato numerico integrato."
type: docs
url: /it/net/aspose.cells/style/custom/
---
## Style.Custom property

Rappresenta la stringa di formato numerico personalizzato di questo oggetto stile. Se il formato numerico personalizzato non è impostato (ad esempio, il formato numerico è incorporato), verrà restituita una stringa vuota "".

```csharp
public string Custom { get; set; }
```

### Osservazioni

La stringa personalizzata restituita è indipendente dalla cultura.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCustomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea e applica un formato data personalizzato
            Style style = workbook.CreateStyle();
            style.Custom = "d-mmm-yy";
            
            cells["A1"].PutValue(new DateTime(2023, 10, 15));
            cells["A1"].SetStyle(style);

            // Visualizza il valore formattato
            Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
            
            // Salva la cartella di lavoro
            workbook.Save("StylePropertyCustomDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


