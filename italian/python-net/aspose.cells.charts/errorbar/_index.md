---
title: classe ErrorBar
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 150
url: /it/python-net/aspose.cells.charts/errorbar/
is_root: false
---
##  classe ErrorBar
Rappresenta la barra di errore delle serie di dati.



**Eredità:** [ErrorBar](/cells/python-net/aspose.cells.charts/errorbar) → 
[Line](/cells/it/python-net/aspose.cells.drawing/line)



Il tipo ErrorBar espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [compound_type](/cells/it/python-net/aspose.cells.charts/errorbar/compound_type) | Specifica il tipo di linea composta|
| [dash_type](/cells/it/python-net/aspose.cells.charts/errorbar/dash_type) | Specifica il tipo di linea tratteggiata|
| [cap_type](/cells/it/python-net/aspose.cells.charts/errorbar/cap_type) | Specifica le maiuscole finali.|
| [join_type](/cells/it/python-net/aspose.cells.charts/errorbar/join_type) | Specifica le estremità di giunzione.|
| [begin_type](/cells/it/python-net/aspose.cells.charts/errorbar/begin_type) |Specifica una freccia per l'inizio di una riga.|
| [end_type](/cells/it/python-net/aspose.cells.charts/errorbar/end_type) | Specifica una freccia per la fine di una riga.|
| [begin_arrow_length](/cells/it/python-net/aspose.cells.charts/errorbar/begin_arrow_length) | Specifica la lunghezza della punta della freccia per l'inizio di una riga.|
| [end_arrow_length](/cells/it/python-net/aspose.cells.charts/errorbar/end_arrow_length) | Specifica la lunghezza della punta della freccia per la fine di una riga.|
| [begin_arrow_width](/cells/it/python-net/aspose.cells.charts/errorbar/begin_arrow_width) | Specifica la larghezza della punta della freccia per l'inizio di una riga.|
| [end_arrow_width](/cells/it/python-net/aspose.cells.charts/errorbar/end_arrow_width) | Specifica la larghezza della punta della freccia per la fine di una riga.|
| [theme_color](/cells/it/python-net/aspose.cells.charts/errorbar/theme_color) | Ottiene e imposta il colore del tema.|
| [color](/cells/it/python-net/aspose.cells.charts/errorbar/color) | Rappresenta il Colore della linea.|
| [transparency](/cells/it/python-net/aspose.cells.charts/errorbar/transparency) | Restituisce o imposta il grado di trasparenza della linea come valore compreso tra 0,0 (opaco) e 1,0 (chiaro).|
| [style](/cells/it/python-net/aspose.cells.charts/errorbar/style) | Rappresenta lo stile della linea.|
| [weight](/cells/it/python-net/aspose.cells.charts/errorbar/weight) | Ottiene o imposta lo [WeightType](/cells/it/python-net/aspose.cells.drawing/weighttype) della riga.|
| [weight_pt](/cells/it/python-net/aspose.cells.charts/errorbar/weight_pt) | Ottiene o imposta lo spessore della linea in unità di punti.|
| [weight_px](/cells/it/python-net/aspose.cells.charts/errorbar/weight_px) | Ottiene o imposta lo spessore della linea in unità di pixel.|
| [formatting_type](/cells/it/python-net/aspose.cells.charts/errorbar/formatting_type) | Ottiene o imposta il tipo di formato.|
| [is_automatic_color](/cells/it/python-net/aspose.cells.charts/errorbar/is_automatic_color) | Indica se il colore della linea viene assegnato automaticamente.|
| [is_visible](/cells/it/python-net/aspose.cells.charts/errorbar/is_visible) | Indica se la linea è visibile.|
| [is_auto](/cells/it/python-net/aspose.cells.charts/errorbar/is_auto) | Indica se questo stile di linea è assegnato automaticamente.|
| [gradient_fill](/cells/it/python-net/aspose.cells.charts/errorbar/gradient_fill) | Rappresenta il riempimento sfumato.|
| [type](/cells/it/python-net/aspose.cells.charts/errorbar/type) |Rappresenta il tipo di importo della barra di errore.|
| [display_type](/cells/it/python-net/aspose.cells.charts/errorbar/display_type) | Rappresenta il tipo di visualizzazione della barra di errore.|
| [amount](/cells/it/python-net/aspose.cells.charts/errorbar/amount) | Rappresenta la quantità di barra di errore.<br/> L'importo deve essere maggiore o uguale a zero.|
| [show_marker_t_top](/cells/it/python-net/aspose.cells.charts/errorbar/show_marker_t_top) | Indica se formattare le barre di errore con un T-top.|
| [plus_value](/cells/it/python-net/aspose.cells.charts/errorbar/plus_value) | Rappresenta l'importo dell'errore positivo quando il tipo di barra di errore è Personalizzato.|
| [minus_value](/cells/it/python-net/aspose.cells.charts/errorbar/minus_value) | Rappresenta l'importo dell'errore negativo quando il tipo di barra di errore è Personalizzato.|



###  Esempi

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, ErrorBarDisplayType, ErrorBarType

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("a1").put_value(2)
cells.get("a2").put_value(5)
cells.get("a3").put_value(3)
cells.get("a4").put_value(6)
cells.get("b1").put_value(4)
cells.get("b2").put_value(3)
cells.get("b3").put_value(6)
cells.get("b4").put_value(7)
cells.get("C1").put_value("Q1")
cells.get("C2").put_value("Q2")
cells.get("C3").put_value("Y1")
cells.get("C4").put_value("Y2")
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 11, 0, 27, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:B4", True)
chart.n_series.category_data = "C1:C4"
for i in range(len(chart.NSeries)):
    aseries = chart.n_series[i]
    aseries.y_error_bar.display_type = ErrorBarDisplayType.MINUS
    aseries.y_error_bar.type = ErrorBarType.FIXED_VALUE
    aseries.y_error_bar.amount = 5

```

###  Guarda anche
* modulo [aspose.cells.charts](..)
* classe [ErrorBar](/cells/it/python-net/aspose.cells.charts/errorbar)
* classe [Line](/cells/it/python-net/aspose.cells.drawing/line)
* classe [WeightType](/cells/it/python-net/aspose.cells.drawing/weighttype)
