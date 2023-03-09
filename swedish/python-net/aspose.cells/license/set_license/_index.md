---
title: set_license metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/license/set_license/
is_root: false
---
##  set_license(license_name) {#str}
Licensierar komponenterna.



```python
def set_license(self, license_name):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| license_name | str |  |
###  Anmärkningar

Försök att hitta licensen på följande platser:


1. Explicit väg.


2. Mappen som innehåller komponentsammansättningen Aspose.


3. Mappen som innehåller klientens anropssammansättning.


4. Mappen som innehåller posten (start) assembly.


5. En inbäddad resurs i klientens anropssammansättning.


**Anmärkningar:** På .NET Compact Framework försöker du hitta licensen endast på dessa platser:


1. Explicit väg.


2. En inbäddad resurs i klientens anropssammansättning.
###  Exempel


I det här exemplet kommer ett försök att göras att hitta en licensfil med namnet MyLicense.lic
 i mappen som innehåller


komponenten, i mappen som innehåller den anropande församlingen,
i mappen för postförsamlingen och sedan i de inbäddade resurserna för den anropande församlingen.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```
Kan vara ett fullständigt eller kort filnamn eller namn på en inbäddad resurs.
Använd en tom sträng för att växla till utvärderingsläge.


##  set_license(stream) {#io.RawIOBase}
Licensierar komponenterna.



```python
def set_license(self, stream):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | En stream som innehåller licensen.|
###  Anmärkningar

Använd den här metoden för att ladda en licens från en stream.
###  Exempel


```python
from aspose.cells import License

license = License()
license.set_license(myStream)

```



###  Se även
* modul [aspose.cells](../../)
* klass [License](/cells/sv/python-net/aspose.cells/license)
