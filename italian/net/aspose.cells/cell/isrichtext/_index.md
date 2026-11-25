---
title: "Cell.IsRichText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Indica se il valore stringa di questa cella è un testo formattato riccamente"
type: docs
url: /it/net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Indica se il valore stringa di questa cella è un testo formattato in rich text.

```csharp
public bool IsRichText()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodIsRichTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una cella con formattazione di testo ricco
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello World");
            
            // Applica la formattazione di testo ricco
            FontSetting boldFont = cell.GetCharacters()[0];
            boldFont.Font.IsBold = true;
            
            FontSetting normalFont = cell.GetCharacters()[6];
            normalFont.Font.IsBold = false;
            
            // Verifica se la cella contiene testo ricco
            bool isRichText = cell.IsRichText();
            Console.WriteLine("Is cell A1 rich text? " + isRichText);
            
            // Salva la cartella di lavoro
            workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


