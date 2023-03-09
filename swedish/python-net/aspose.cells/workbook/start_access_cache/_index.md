---
title: start_access_cache metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 380
url: /sv/python-net/aspose.cells/workbook/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
Startar sessionen som använder cachar för att komma åt data.



```python
def start_access_cache(self, opts):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/sv/python-net/aspose.cells/accesscacheoptions) | alternativ för dataåtkomst|
###  Anmärkningar

Om cachen för specificerad dataåtkomst kräver att vissa datamodeller i kalkylbladet är "skrivskyddade",
då kommer motsvarande datamodeller i varje kalkylblad i denna arbetsbok att tas som "skrivskyddad"
och användaren ska inte ändra någon av dem.


Efter att ha avslutat åtkomsten till uppgifterna bör [Workbook.close_access_cache(opts)](/cells/sv/python-net/aspose.cells/workbook/close_access_cache)
anropas med samma alternativ för att rensa alla cachar och återställa normalt åtkomstläge.


###  Se även
* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
