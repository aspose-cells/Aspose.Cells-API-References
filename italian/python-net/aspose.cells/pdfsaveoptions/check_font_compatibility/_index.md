---
title: check_font_compatibility proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 80
url: /it/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility/
is_root: false
---
##  check_font_compatibility proprietà

Indica se controllare la compatibilità dei caratteri per ogni carattere nel testo.

###  Osservazioni

Il valore predefinito è vero.
Disattivare questa proprietà può fornire prestazioni migliori.
Ma quando il carattere predefinito o specificato di testo/carattere non può essere utilizzato per visualizzarlo,
caratteri illeggibili (come il blocco) potrebbero verificarsi nel pdf generato.
Per tale situazione l'utente dovrebbe mantenere questa proprietà come true in modo che
font alternativo può essere ricercato e utilizzato invece per rendere il testo;
###  Definizione:
```python
@property
def check_font_compatibility(self):
    ...
@check_font_compatibility.setter
def check_font_compatibility(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [PdfSaveOptions](/cells/it/python-net/aspose.cells/pdfsaveoptions)
