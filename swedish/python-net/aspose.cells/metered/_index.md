---
title: Metered klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1050
url: /sv/python-net/aspose.cells/metered/
is_root: false
---
##  Metered klass
Tillhandahåller metoder för att ställa in mätnycklar.



Typen Metered avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [Metered()](/cells/sv/python-net/aspose.cells/metered/__init__/#) | Initierar en ny instans av den här klassen.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/sv/python-net/aspose.cells/metered/set_metered_key/#str-str) | Ställer in mätta offentliga och privata nycklar.<br/>Om du köper mätlicens, när du startar ansökan, ska denna API kallas, normalt räcker det. Du bör regelbundet kontrollera licensstatusen, om det är utvärderingsstatus, ring detta API igen.|
| [get_consumption_quantity()](/cells/sv/python-net/aspose.cells/metered/get_consumption_quantity/#) | Får förbrukningsfilstorlek|
| [get_consumption_credit()](/cells/sv/python-net/aspose.cells/metered/get_consumption_credit/#) | Får konsumtionskredit|



###  Exempel

I det här exemplet kommer ett försök att göras att ställa in mätta publika och privata nycklar


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Se även
* modul [aspose.cells](..)
