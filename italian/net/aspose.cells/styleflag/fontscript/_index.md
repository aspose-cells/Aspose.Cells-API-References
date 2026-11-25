---
title: "StyleFlag.FontScript"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione dello script del carattere"
type: docs
url: /it/net/aspose.cells/styleflag/fontscript/
---
## StyleFlag.FontScript property

L'impostazione dello script del carattere sarà applicata.

```csharp
public bool FontScript { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontScriptDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta del testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Crea un oggetto stile e imposta lo script del carattere su pedice
            Style style = workbook.CreateStyle();
            style.Font.IsSubscript = true;

            // Crea un flag di stile e abilita il flag FontScript
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontScript = true;

            // Applica lo stile alla cella con il flag di stile
            cell.SetStyle(style, styleFlag);

            // Visualizza lo stato corrente dello script del carattere
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Modifica lo script del carattere in apice
            style.Font.IsSubscript = false;
            style.Font.IsSuperscript = false;
            cell.SetStyle(style, styleFlag);

            // Visualizza lo stato aggiornato dello script del carattere
            Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Salva la cartella di lavoro
            workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


