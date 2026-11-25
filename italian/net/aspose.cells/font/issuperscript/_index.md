---
title: "Font.IsSuperscript"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene o imposta un valore che indica se il carattere è in apice"
type: docs
url: /it/net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Ottiene o imposta un valore che indica se il carattere è apice.

```csharp
public bool IsSuperscript { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSuperscriptDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi testo alla cella A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Normal Text Superscript Text");
            
            // Formatta parte del testo come apice
            FontSetting setting = cell.Characters(12, 11);
            setting.Font.IsSuperscript = true;
            
            // Salva la cartella di lavoro
            workbook.Save("FontIsSuperscriptDemo.xlsx");
            
            // Verifica l'impostazione del apice
            Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


