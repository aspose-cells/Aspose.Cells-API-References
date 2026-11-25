---
title: "StyleFlag.FontUnderline"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione della sottolineatura del carattere verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/fontunderline/
---
## StyleFlag.FontUnderline property

L'impostazione di sottolineatura del carattere sarà applicata.

```csharp
public bool FontUnderline { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontUnderlineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta del testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with Underline");

            // Crea un oggetto stile e imposta la sottolineatura del carattere
            Style style = workbook.CreateStyle();
            style.Font.Underline = FontUnderlineType.Single;

            // Crea un flag di stile e abilita il flag di sottolineatura del carattere
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontUnderline = true;

            // Applica lo stile alla cella con il flag di stile
            cell.SetStyle(style, styleFlag);

            // Mostra lo stato attuale della sottolineatura
            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Cambia il tipo di sottolineatura in doppio
            style.Font.Underline = FontUnderlineType.Double;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Salva la cartella di lavoro
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


