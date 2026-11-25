---
title: "StyleFlag.FontStrike"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione di barrato del carattere"
type: docs
url: /it/net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

L'impostazione di barrato del carattere sarà applicata.

```csharp
public bool FontStrike { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta del testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Crea un oggetto stile e imposta FontStrike a true
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // Crea un flag di stile e abilita il flag FontStrike
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // Applica lo stile alla cella con il flag di stile
            cell.SetStyle(style, styleFlag);

            // Mostra lo stato corrente di FontStrike
            Console.WriteLine("FontStrike applied: " + cell.GetStyle().Font.IsStrikeout);

            // Crea un'altra cella per dimostrare testo non barrato
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");
            styleFlag.FontStrike = false;

            cell2.SetStyle(style, styleFlag);
            Console.WriteLine("FontStrike applied: " + cell2.GetStyle().Font.IsStrikeout);

            // Salva la cartella di lavoro per vedere gli effetti
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


