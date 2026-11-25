---
title: "FillFormat.SetOneColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FillFormat. Imposta il riempimento specificato a un gradiente a un colore. Valido solo per Excel 2007"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/setonecolorgradient/
---
## FillFormat.SetOneColorGradient method

Imposta il riempimento specificato a un gradiente a un colore. Valido solo per Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colore | Color | Un colore di gradiente. |
| grado | Double | Il grado del gradiente. Può essere un valore da 0.0 (scuro) a 1.0 (chiaro). |
| stile | GradientStyleType | Stile di sfumatura del gradiente. |
| variant | Int32 | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradient del dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Applica riempimento a gradiente alla prima serie
            Series series = chart.NSeries[0];
            series.IsColorVaried = false;
            
            // Dimostra SetOneColorGradient con parametri specifici
            series.Area.FillFormat.SetOneColorGradient(
                Color.FromArgb(0, 236, 102, 102), // Color
                0.9,                              // Transparency
                Aspose.Cells.Drawing.GradientStyleType.DiagonalDown,    // Gradient style
                2);                                // Variant

            // Salva la cartella di lavoro
            workbook.Save("FillFormat_SetOneColorGradient_Output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


