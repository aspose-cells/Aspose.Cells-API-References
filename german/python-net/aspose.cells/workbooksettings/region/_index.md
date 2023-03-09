---
title: region Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 520
url: /de/python-net/aspose.cells/workbooksettings/region/
is_root: false
---
##  region Eigentum

Ruft die regionalen Einstellungen für Arbeitsmappen ab oder legt diese fest.

###  Bemerkungen

1. Regionale Einstellungen, die von der Komponente Aspose.Cells für eine Arbeitsmappe verwendet werden, die aus einer Vorlagendatei geladen wurde:
i) Für eine XLS-Datei sind Felder für regionale Einstellungen definiert und MS Excel speichert regionale Einstellungsdaten in der Datei, wenn die XLS-Datei gespeichert wird.
Wir verwenden also die gespeicherte region in der Vorlagendatei für die Arbeitsmappe.
Wenn Sie die in der Datei XLS gespeicherte region nicht verwenden möchten, setzen Sie sie bitte nach dem Laden der Vorlagendatei auf die erwartete zurück (z. B. CountryCode.Default).
Und wir speichern den benutzerdefinierten Wert (mit dieser Methode) auch in der Datei, wenn wir eine XLS-Datei speichern.
ii) Für andere Dateiformate wie XLSX, XLSB usw. ist kein Feld für regionale Einstellungen in der Dateiformatspezifikation definiert.
Daher verwenden wir die regionalen Einstellungen der Anwendungsumgebung für die Arbeitsmappe.
Und der vom Benutzer angegebene Wert (durch diese Methode) kann für die generierten Dateien mit diesen Dateiformaten nicht beibehalten werden.
2. Für den Ansichtseffekt in MS Excel:
Die hier vorgenommenen regionalen Einstellungen können nur zur Laufzeit mit der Komponente Aspose.Cells wirksam werden und nicht beim Anzeigen der generierten Datei mit MS Excel.
Auch für die generierte XLS-Datei, in der die angegebenen Ländereinstellungsdaten gespeichert wurden, wenn Sie sie mit MS Excel anzeigen/bearbeiten,
die verwendete region, um die Formatierung durch MS Excel durchzuführen, ist immer die standardmäßige regionale Einstellung der Umgebung, in der MS Excel ausgeführt wird,
nicht die in der Datei gespeicherte.
###  Definition:
```python
@property
def region(self):
    ...
@region.setter
def region(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [CountryCode](/cells/de/python-net/aspose.cells/countrycode)
* Klasse [WorkbookSettings](/cells/de/python-net/aspose.cells/workbooksettings)
