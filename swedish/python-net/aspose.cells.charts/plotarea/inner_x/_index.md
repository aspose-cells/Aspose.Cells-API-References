---
title: inner_x fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 170
url: /sv/python-net/aspose.cells.charts/plotarea/inner_x/
is_root: false
---
##  inner_x fastighet

Hämtar eller hämtar x-koordinaten för det övre övre hörnet av plotområdet i enheter på 1/4000 av diagramytan.

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
def inner_x(self):
    ...
@inner_x.setter
def inner_x(self, value):
    ...
```

###  Se även
* modul [aspose.cells.charts](../../)
* klass [PlotArea](/cells/sv/python-net/aspose.cells.charts/plotarea)
