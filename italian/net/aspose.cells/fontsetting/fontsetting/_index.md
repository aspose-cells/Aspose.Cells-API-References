---
title: "FontSetting.FontSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore FontSetting."
type: docs
url: /it/net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 |  |
| lunghezza | Int32 |  |
| fogli | WorksheetCollection |  |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi testo di esempio alla cella
            worksheet.Cells["A1"].PutValue("Hello World");
            
            // Crea impostazione del carattere per i primi 5 caratteri (0-4) in tutti i fogli di lavoro
            FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
            
            // Applicare la formattazione
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Size = 14;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


