---
title: "FillFormat.SetPresetColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FillFormat. Imposta il riempimento specificato a un gradiente presetcolor. Valido solo per Excel 2007"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/setpresetcolorgradient/
---
## FillFormat.SetPresetColorGradient method

Imposta il riempimento specificato a un gradiente con colore predefinito. Valido solo per Excel 2007.

```csharp
public void SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, 
    int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| presetColor | GradientPresetType | Tipo di colore predefinito |
| stile | GradientStyleType | Stile di sfumatura del gradiente. |
| variant | Int32 | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradient del dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetPresetColorGradientWithGradientPresetTypeGradientStylDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Item {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Crea grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 8, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Applica riempimento gradiente
            FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
            fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);

            // Salva la cartella di lavoro
            workbook.Save("SetPresetColorGradientDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientPresetType](../../gradientpresettype/)
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


