---
title: culture_custom proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 170
url: /it/python-net/aspose.cells/style/culture_custom/
is_root: false
---
##  culture_custom proprietà

Ottiene e imposta la stringa del modello dipendente dalle impostazioni cultura per il formato numerico.
Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null.
Se il formato del numero è incorporato, verrà restituita la stringa del modello corrispondente al numero incorporato.

###  Osservazioni

Per il formato numerico integrato, sia il contenuto del pattern (ad esempio, un formato data integrato è "m/g/a" per alcune impostazioni locali,
ma per alcune altre localizzazioni diventa "d/m/y") e l'identificatore di formato (come,
alcune impostazioni locali utilizzano caratteri diversi da "y" per rappresentare la parte dell'anno per la formattazione della data)
dipendono dalla cultura;
Per il formato personalizzato specificato dall'utente, solo gli identificatori di formato vengono modificati in base alla cultura,
altre parti del modello di formattazione non verranno modificate.
###  Definizione:
```python
@property
def culture_custom(self):
    ...
@culture_custom.setter
def culture_custom(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Style](/cells/it/python-net/aspose.cells/style)
