---
title: "FontConfigs.SetFontFolder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontConfigs. Imposta la cartella dei font"
type: docs
url: /it/net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Imposta la cartella dei caratteri

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolder | String | La cartella che contiene i font TrueType. |
| ricorsivo | Booleano | Determina se scansionare o meno le sottocartelle. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi del testo alla cella A1
            worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
            
            // Imposta la cartella dei font personalizzata e specifica se includere le sottocartelle
            FontConfigs.SetFontFolder("Fonts", true);
            
            // Applica uno stile di font che potrebbe utilizzare i font dalla cartella personalizzata
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Salva la cartella di lavoro in PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Vedi anche

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


