---
title: update_linked_data_source Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 410
url: /de/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
Wenn diese Arbeitsmappe externe Links zu anderen Datenquellen enthält,
Aspose.Cells wird versuchen, die neuesten Daten abzurufen.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| external_workbooks | list | Externe Arbeitsmappen werden von dieser Arbeitsmappe referenziert.<br/>Wenn es null ist, werden wir die extern verlinkten Dateien direkt öffnen.<br/> Wenn es nicht null ist,<br/>wir werden zuerst prüfen, ob der externe Link im Array ist;<br/> Wenn nicht, öffnen wir die extern verlinkten Dateien erneut.|
###  Bemerkungen

Wenn die Methode nicht vor dem Berechnen von Formeln aufgerufen wird,
Aspose.Cells verwendet die vorherigen Informationen (in der Datei zwischengespeichert);
 Bitte legen Sie CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath fest.
Und bitte setzen Sie Workbook.FilePath, wenn diese Arbeitsmappe aus einem Stream stammt,
andernfalls konnte Aspose.Cells manchmal den vollständigen Pfad des externen Links nicht abrufen.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
