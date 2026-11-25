---
title: "StyleFlag.HideFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. L'impostazione Hide formula verrà applicata"
type: docs
url: /it/net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

L'impostazione di nascondi formula sarà applicata.

```csharp
public bool HideFormula { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell a1 = worksheet.Cells["A1"];
            // Aggiungi una formula alla cella A1
            a1.Formula = "=1+2";
            a1.Value = 3; // Display value

            // Crea un flag di stile con HideFormula impostato su true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // Crea uno stile e imposta IsFormulaHidden su true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // Applica lo stile alla cella A1 con il flag di stile
            a1.SetStyle(style, styleFlag);

            // Proteggi il foglio di lavoro per vedere l'effetto di HideFormula
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // Salva la cartella di lavoro
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // Verifica che la formula sia nascosta
            Console.WriteLine("Formula in A1: " + a1.Formula);
            Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


