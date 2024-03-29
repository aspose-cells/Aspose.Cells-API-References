---
title: X
second_title: Aspose.Cells för .NET API-referens
description: Hämtar eller hämtar x-koordinaten för det övre vänstra hörnet av markeringsrutan för plot-area i enheter på 1/4000 av sjökortsytan.
type: docs
weight: 80
url: /sv/net/aspose.cells.charts/plotarea/x/
---
## PlotArea.X property

Hämtar eller hämtar x-koordinaten för det övre vänstra hörnet av markeringsrutan för plot-area i enheter på 1/4000 av sjökortsytan.

```csharp
public override int X { get; set; }
```

### Anmärkningar

Avgränsningsrutan för plot-area inkluderar plot-arean, tick marks(tick labels) och en liten ram runt tick marks. Om värdet inte skapas av MS Excel, vänligen anropa Chart.Calculate() metoden innan du anropar den här metoden .

De **X** , **Y** , **Bredd** och **Höjd** av **PlotArea** representerar plottområdet begränsningsrutan som inkluderar plottområdet, bockmarkeringar (tick-etiketter) och en liten kant runt bockmarkeringarna. Om du vill få verklig storlek på tomtytan bör du ringa **InnerX** , **InreY** , **InnerWidth** och  **Innerhöjd** egenskaper.

För excel 2007 eller senare är standardvärdet noll. du bör anropa få värdet efter att ha anropat Chart.Calculate().

### Se även

* class [PlotArea](../../plotarea)
* namnutrymme [Aspose.Cells.Charts](../../plotarea)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
