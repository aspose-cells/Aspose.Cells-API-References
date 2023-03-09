---
title: inner_height proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 150
url: /it/python-net/aspose.cells.charts/plotarea/inner_height/
is_root: false
---
##  inner_height proprietà

Ottiene o imposta l'altezza dell'area del tracciato in unità di 1/4000 dell'area del grafico.

###  Osservazioni

Il riquadro di delimitazione dell'area del tracciato include l'area del tracciato, i segni di graduazione (etichette di graduazione) e un piccolo bordo attorno ai segni di graduazione.
 Se il valore non viene creato da MS Excel, chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.


 IL**X** , **Y** , **Larghezza** E**Altezza** Di**Area del grafico** rappresenta l'area del grafico
 Un rettangolo di delimitazione che include l'area del tracciato, i segni di graduazione (etichette di graduazione) e un piccolo bordo attorno ai segni di graduazione.
 Se vuoi ottenere la dimensione effettiva dell'area del tracciato, dovresti chiamare**X interna** , **Y interiore** , **Larghezza interna** E
**Altezza interna** proprietà.


Per Excel 2007 o versioni successive, il valore predefinito è zero.
###  Definizione:
```python
@property
def inner_height(self):
    ...
@inner_height.setter
def inner_height(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.charts](../../)
* classe [PlotArea](/cells/it/python-net/aspose.cells.charts/plotarea)
