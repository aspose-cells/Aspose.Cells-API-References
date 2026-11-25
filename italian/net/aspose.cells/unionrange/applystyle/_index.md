---
title: "UnionRange.ApplyStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnionRange. Applica formati per un intero intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/applystyle/
---
## UnionRange.ApplyStyle method

Applica formati a un intero intervallo.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stile | Stile | L'oggetto stile che verrà applicato. |
| flag | StyleFlag | Flag che indicano le proprietà di formattazione applicate. |

### Osservazioni

Ogni cella in questo intervallo conterrà un oggetto [`Style`](../../style/). Quindi questo è un metodo che consuma molta memoria. Si prega di usarlo con attenzione.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo di unione che copre le celle A1 a B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "More Data";

            try
            {
                // Crea uno stile con formattazione specifica
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.Font.Color = Color.Red;
                style.ForegroundColor = Color.LightBlue;
                style.Pattern = BackgroundType.Solid;
                style.HorizontalAlignment = TextAlignmentType.Center;

                // Crea un StyleFlag per specificare quali proprietà applicare
                StyleFlag flag = new StyleFlag();
                flag.FontBold = true;
                flag.FontColor = true;
                flag.CellShading = true;
                flag.HorizontalAlignment = true;

                // Chiama ApplyStyle con i parametri stile e flag
                unionRange.ApplyStyle(style, flag);

                Console.WriteLine("ApplyStyle method called successfully");
                Console.WriteLine($"Applied style to range: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ApplyStyle: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("UnionRangeMethodApplyStyleWithStyleStyleFlagDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


