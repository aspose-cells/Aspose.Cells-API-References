---
title: "Font.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta il nome del Font"
type: docs
url: /it/net/aspose.cells/font/name/
---
## Font.Name property

Ottiene o imposta il nome del [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Osservazioni

Se questa proprietà viene utilizzata per impostare il nome del carattere, il [`SchemeType`](../schemetype/) verrà aggiornato a None

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al foglio di lavoro predefinito e alle celle
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crea e modifica uno stile con le proprietà del carattere
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // Dimostra l'uso della proprietà Name
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // Applica lo stile a una cella
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


