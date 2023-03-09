---
title: width fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 260
url: /sv/python-net/aspose.cells.charts/plotarea/width/
is_root: false
---
##  width fastighet

Hämtar eller ställer in width för plot-area avgränsningsruta i enheter på 1/4000 av sjökortsytan.

###  Anmärkningar

Avgränsningsrutan för plottarea inkluderar tomtområdet, bockmarkeringar (tick-etiketter) och en liten ram runt bockmarkeringarna.
 Om värdet inte skapas av MS Excel, anropa metoden Chart.Calculate() innan du anropar den här metoden.


 De**X** , **Y** , **Bredd** och**Höjd** av**Tomtområde** representerar tomtområdet
 En avgränsningsruta som inkluderar plotområdet, bockmarkeringar (tick-etiketter) och en liten kant runt bockmarkeringarna.
 Vill du få verklig storlek på tomtarea ska du ringa**Inre X** , **Inre Y** , **Inre bredd** och
**Inre höjd** egenskaper.


För excel 2007 eller senare är standardvärdet noll.
###  Definition:
```python
@property
def width(self):
    ...
@width.setter
def width(self, value):
    ...
```

###  Se även
* modul [aspose.cells.charts](../../)
* klass [PlotArea](/cells/sv/python-net/aspose.cells.charts/plotarea)
