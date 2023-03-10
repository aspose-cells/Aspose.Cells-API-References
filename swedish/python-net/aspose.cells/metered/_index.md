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
Ger metoder för att ställa in mätt nyckel.



Typen Metered avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [Metered()](/cells/sv/python-net/aspose.cells/metered/__init__/#) | Initierar en ny instans av den här klassen.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/sv/python-net/aspose.cells/metered/set_metered_key/#str-str) | Ställer in mätt offentlig och privat nyckel.<br/>Om du köper mätlicens, när du startar ansökan, bör denna API kallas, normalt räcker detta. Men om alltid misslyckas med att ladda upp förbrukningsdata och överskrider 24 timmar, kommer licensen att ställas in på utvärderingsstatus, för att undvika sådana fall bör du regelbundet kontrollera licensstatusen, om det är utvärderingsstatus, ring detta API igen.|
| [get_consumption_quantity()](/cells/sv/python-net/aspose.cells/metered/get_consumption_quantity/#) | Får förbrukningsfilstorlek|
| [get_consumption_credit()](/cells/sv/python-net/aspose.cells/metered/get_consumption_credit/#) | Får konsumtionskredit|



###  Exempel

I det här exemplet kommer ett försök att göras att ställa in mätt offentlig och privat nyckel


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Se även
* modul [aspose.cells](..)
