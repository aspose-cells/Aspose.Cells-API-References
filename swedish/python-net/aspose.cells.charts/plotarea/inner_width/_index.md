---
title: inner_width fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 160
url: /sv/python-net/aspose.cells.charts/plotarea/inner_width/
is_root: false
---
##  inner_width fastighet

Hämtar eller ställer in bredden på plotområdet i enheter på 1/4000 av diagramytan.

###  Anmärkningar

Avgränsningsrutan för plottarea inkluderar tomtområdet, bockmarkeringar (tick-etiketter) och en liten ram runt bockmarkeringarna.
 Om värdet inte skapas av MS Excel, anropa metoden Chart.Calculate() innan du anropar den här metoden.


 De**X** , **Y** , **Bredd** och**Höjd** av**PlotArea** representerar tomtområdet
 begränsningsruta som inkluderar tomtområdet, bockmarkeringar (tick-etiketter) och en liten kant runt bockmarkeringarna.
 Vill du få verklig storlek på tomtarea ska du ringa**InnerX** , **InreY** , **InnerWidth** och
**Innerhöjd** egenskaper.


För excel 2007 eller senare är standardvärdet noll. du bör anropa få värdet efter att ha anropat Chart.Calculate().
###  Definition:
```python
@property
def inner_width(self):
    ...
@inner_width.setter
def inner_width(self, value):
    ...
```

###  Se även
* modul [aspose.cells.charts](../../)
* klass [PlotArea](/cells/sv/python-net/aspose.cells.charts/plotarea)
