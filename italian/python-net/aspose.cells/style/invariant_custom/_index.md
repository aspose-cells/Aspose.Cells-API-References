---
title: invariant_custom proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 260
url: /it/python-net/aspose.cells/style/invariant_custom/
is_root: false
---
##  invariant_custom proprietà

Ottiene la stringa del modello indipendente dalle impostazioni cultura per il formato numerico.
Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null.
Se il formato del numero è incorporato, verrà restituita la stringa del modello corrispondente al numero incorporato.

###  Osservazioni

Per i formati numerici incorporati, il contenuto del modello restituito è ancora dipendente dalla cultura,
ad esempio, per alcune locali restituisce "m/d/y" e per alcune altre locali restituisce "d/m/y".
La differenza rispetto a [Style.culture_custom](/cells/it/python-net/aspose.cells/style#culture_custom) è (questo è anche ciò che significa indipendente dalla cultura):
gli identificatori di formato e i separatori sono mantenuti come standard, ad esempio '/' verrà sempre utilizzato come separatore di data e ora
e "y" sarà sempre usato come parte dell'"anno", indipendentemente da quale altro carattere speciale sia usato per il locale specifico.
###  Definizione:
```python
@property
def invariant_custom(self):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Style](/cells/it/python-net/aspose.cells/style)
