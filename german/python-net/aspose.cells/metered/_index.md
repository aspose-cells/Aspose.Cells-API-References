---
title: Metered Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1050
url: /de/python-net/aspose.cells/metered/
is_root: false
---
##  Metered Klasse
Stellt Methoden zum Festlegen von getakteten Schlüsseln bereit.



Der Typ Metered macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [Metered()](/cells/de/python-net/aspose.cells/metered/__init__/#) | Initialisiert eine neue Instanz dieser Klasse.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/de/python-net/aspose.cells/metered/set_metered_key/#str-str) | Legt gemessene öffentliche und private Schlüssel fest.<br/>Wenn Sie eine kostenpflichtige Lizenz erwerben, sollte beim Start der Anwendung diese API angerufen werden, normalerweise reicht dies. Sie sollten den Lizenzstatus regelmäßig überprüfen, wenn es sich um einen Evaluierungsstatus handelt, rufen Sie diese API erneut an.|
| [get_consumption_quantity()](/cells/de/python-net/aspose.cells/metered/get_consumption_quantity/#) | Ruft die Größe der Verbrauchsdatei ab|
| [get_consumption_credit()](/cells/de/python-net/aspose.cells/metered/get_consumption_credit/#) | Konsumguthaben bekommt|



###  Beispiele

In diesem Beispiel wird versucht, getaktete öffentliche und private Schlüssel zu setzen


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Siehe auch
* Modul [aspose.cells](..)
