---
title: y fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 280
url: /sv/python-net/aspose.cells.charts/plotarea/y/
is_root: false
---
##  y fastighet

Hämtar eller hämtar y-koordinaten för det övre övre hörnet av gränsrutan för plot-area i enheter på 1/4000 av kartytan.

###  Anmärkningar

Avgränsningsrutan för plottarea inkluderar tomtområdet, bockmarkeringar (tick-etiketter) och en liten ram runt bockmarkeringarna.
Om värdet inte skapas av MS Excel, anropa metoden Chart.Calculate() innan du anropar den här metoden.


 De**X** , **Y** , **Bredd** och**Höjd** av**PlotArea** representerar tomtområdet
 begränsningsruta som inkluderar tomtområdet, bockmarkeringar (tick-etiketter) och en liten kant runt bockmarkeringarna.
 Vill du få verklig storlek på tomtarea ska du ringa**InnerX** , **InreY** , **InnerWidth** och
**InnerHeight** egenskaper.


För excel 2007 eller senare är standardvärdet noll. du bör anropa få värdet efter att ha anropat Chart.Calculate().
###  Definition:
```python
@property
def y(self):
    ...
@y.setter
def y(self, value):
    ...
```

###  Se även
* modul [aspose.cells.charts](../../)
* klass [PlotArea](/cells/sv/python-net/aspose.cells.charts/plotarea)
