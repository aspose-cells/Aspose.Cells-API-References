---
title: multi_thread_reading Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1200
url: /de/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
##  multi_thread_reading Eigentum

Ruft ab oder legt fest, ob das Zellendatenmodell Multi-Thread-Lesen unterstützen soll.
Der Standardwert dieser Eigenschaft ist false.

###  Bemerkungen

Wenn es mehrere Threads zum gleichzeitigen Lesen von Row/Cell-Objekten in dieser Sammlung gibt,
diese Eigenschaft sollte auf true gesetzt werden, andernfalls kann es zu unerwarteten Ergebnissen kommen.
Die Unterstützung von Multi-Thread-Lesen kann die Leistung für den Zugriff auf Row/Cell-Objekte aus dieser Sammlung beeinträchtigen.
Bitte beachten Sie, dass einige Funktionen kein Multi-Thread-Lesen unterstützen,
wie Formatierung von Werten (durch [Cell.string_value](/cells/de/python-net/aspose.cells/cell#string_value), [Cell.display_string_value](/cells/de/python-net/aspose.cells/cell#display_string_value), .etc.).
Selbst wenn diese Eigenschaft auf „true“ gesetzt ist, können diese APIs also immer noch unerwartete Ergebnisse für das Multi-Thread-Lesen liefern.
###  Definition:
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cells](/cells/de/python-net/aspose.cells/cells)
