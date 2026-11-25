---
title: "ShapeCollection.AddTextEffectInChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Inserisce un oggetto WordArt nel grafico"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
## ShapeCollection.AddTextEffectInChart method

Inserisce un oggetto WordArt al grafico.

```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName, 
    int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| effetto | MsoPresetTextEffect | Il tipo di effetto di testo predefinito mso. |
| testo | String | Il testo WordArt. |
| fontName | String | Il nome del carattere. |
| dimensione | Int32 | La dimensione del carattere |
| fontBold | Booleano | Indica se il carattere è in grassetto. |
| fontItalic | Booleano | Indica se il carattere è in corsivo. |
| alto | Int32 | Rappresenta lo spostamento verticale della forma dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| sinistra | Int32 | Rappresenta lo spostamento verticale della forma dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| altezza | Int32 | Rappresenta l'altezza della forma, in unità di 1/4000 dell'area del grafico. |
| larghezza | Int32 | Rappresenta la larghezza della forma, in unità di 1/4000 dell'area del grafico. |

### Valore di ritorno

Restituisce un oggetto Shape che rappresenta il nuovo oggetto WordArt.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectInChartWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // Aggiungi WordArt al grafico
            Shape wordart = chart.Shapes.AddTextEffectInChart(
                MsoPresetTextEffect.TextEffect2,
                "SAMPLE TEXT", 
                "Arial Black", 
                36, 
                false, 
                false,
                100,  // Left position
                100,  // Top position
                300,  // Width
                200); // Height
                
            // Personalizza l'aspetto di WordArt
            wordart.FillFormat.Transparency = 0.7;
            wordart.LineFormat.IsVisible = false;
            
            // Salva la cartella di lavoro
            workbook.Save("WordArtInChart.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


