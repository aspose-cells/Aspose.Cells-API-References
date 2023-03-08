---
title: start_access_cache Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 380
url: /de/python-net/aspose.cells/workbook/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
Startet die Sitzung, die Caches verwendet, um auf Daten zuzugreifen.



```python
def start_access_cache(self, opts):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/de/python-net/aspose.cells/accesscacheoptions) | Möglichkeiten des Datenzugriffs|
###  Bemerkungen

Wenn der Cache des angegebenen Datenzugriffs erfordert, dass einige Datenmodelle im Arbeitsblatt "schreibgeschützt" sind,
dann werden entsprechende Datenmodelle in jedem Arbeitsblatt in dieser Arbeitsmappe als "schreibgeschützt" betrachtet.
und der Benutzer sollte keine davon ändern.


Nach Abschluss des Zugriffs auf die Daten sollte [Workbook.close_access_cache(opts)](/cells/de/python-net/aspose.cells/workbook/close_access_cache)
mit denselben Optionen aufgerufen werden, um alle Caches zu löschen und den normalen Zugriffsmodus wiederherzustellen.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
