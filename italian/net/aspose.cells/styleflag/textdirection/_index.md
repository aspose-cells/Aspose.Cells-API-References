---
title: "StyleFlag.TextDirection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione della direzione del testo"
type: docs
url: /it/net/aspose.cells/styleflag/textdirection/
---
## StyleFlag.TextDirection property

L'impostazione della direzione del testo sarà applicata.

```csharp
public bool TextDirection { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla cella A1 e imposta del testo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with TextDirection");

            // Crea uno stile e imposta la direzione del testo
            Style style = workbook.CreateStyle();
            style.TextDirection = TextDirectionType.Context;

            // Crea un flag di stile e abilita il flag TextDirection
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TextDirection = true;

            // Applica lo stile alla cella con il flag di stile
            cell.SetStyle(style, styleFlag);

            // Mostra la direzione del testo corrente
            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Cambia la direzione del testo e applica nuovamente
            style.TextDirection = TextDirectionType.LeftToRight;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Salva la cartella di lavoro
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


