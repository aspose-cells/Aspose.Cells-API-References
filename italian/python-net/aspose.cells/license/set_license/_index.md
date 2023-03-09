---
title: metodo set_license
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/license/set_license/
is_root: false
---
##  set_license(license_name) {#str}
Concede in licenza il componente.



```python
def set_license(self, license_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| license_name | str |  |
###  Osservazioni

Tenta di trovare la licenza nelle seguenti posizioni:


1. Percorso esplicito.


2. La cartella che contiene l'assieme del componente Aspose.


3. La cartella che contiene l'assembly chiamante del client.


4. La cartella che contiene l'assembly della voce (avvio).


5. Una risorsa incorporata nell'assembly chiamante del client.


**Nota:** Nel Compact Framework .NET, tenta di trovare la licenza solo in queste posizioni:


1. Percorso esplicito.


2. Una risorsa incorporata nell'assembly chiamante del client.
###  Esempio


In questo esempio, verrà effettuato un tentativo di trovare un file di licenza denominato MyLicense.lic
 nella cartella che contiene


il componente, nella cartella che contiene l'assembly chiamante,
nella cartella dell'assembly di ingresso e quindi nelle risorse incorporate dell'assembly chiamante.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```
Può essere un nome file completo o breve o il nome di una risorsa incorporata.
Utilizzare una stringa vuota per passare alla modalità di valutazione.


##  set_license(stream) {#io.RawIOBase}
Concede in licenza il componente.



```python
def set_license(self, stream):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| stream | io.RawIOBase | Un flusso che contiene la licenza.|
###  Osservazioni

Utilizzare questo metodo per caricare una licenza da un flusso.
###  Esempio


```python
from aspose.cells import License

license = License()
license.set_license(myStream)

```



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [License](/cells/it/python-net/aspose.cells/license)
