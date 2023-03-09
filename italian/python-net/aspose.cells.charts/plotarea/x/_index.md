---
title: x proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 270
url: /it/python-net/aspose.cells.charts/plotarea/x/
is_root: false
---
##  x proprietà

Ottiene o ottiene la coordinata x dell'angolo superiore sinistro del riquadro di delimitazione dell'area del grafico in unità di 1/4000 dell'area del grafico.

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
def x(self):
    ...
@x.setter
def x(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.charts](../../)
* classe [PlotArea](/cells/it/python-net/aspose.cells.charts/plotarea)
