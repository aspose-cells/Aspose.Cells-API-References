---
title: metodo get_style
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells/row/get_style/
is_root: false
---
##  get_style() {#}
Ottiene lo stile di questa riga.



```python
def get_style(self):
    ...
```


###  Osservazioni

La modifica diretta dell'oggetto di stile restituito non ha alcun effetto per questa riga o per qualsiasi cella in questa riga.
Devi chiamare il metodo [Row.apply_style(style, flag)](/cells/it/python-net/aspose.cells/row/apply_style) o [Row.set_style(style)](/cells/it/python-net/aspose.cells/row/set_style)
per applicare la modifica a questa riga.

Lo stile della riga è lo stile che verrà ereditato dalle celle in questa riga (quelle celle che non hanno impostazioni di stile personalizzate,
come le celle esistenti per le quali non è stato impostato lo stile in modo esplicito o quelle per le quali non è stata creata un'istanza)


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Row](/cells/it/python-net/aspose.cells/row)
