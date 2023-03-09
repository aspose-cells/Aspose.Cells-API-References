---
title: classe Metered
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1050
url: /it/python-net/aspose.cells/metered/
is_root: false
---
##  classe Metered
Fornisce metodi per impostare la chiave misurata.



Il tipo Metered espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [Metered()](/cells/it/python-net/aspose.cells/metered/__init__/#) | Inizializza una nuova istanza di questa classe.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/it/python-net/aspose.cells/metered/set_metered_key/#str-str) | Imposta la chiave pubblica e privata misurata.<br/> Se acquisti una licenza a consumo, quando avvii l'applicazione, dovrebbe essere chiamato questo API, normalmente, questo è sufficiente. Tuttavia, se non riesci sempre a caricare i dati di consumo e superi le 24 ore, la licenza verrà impostata sullo stato di valutazione, per evitare tale caso, dovresti controllare regolarmente lo stato della licenza, se è lo stato di valutazione, chiama di nuovo questo API.|
| [get_consumption_quantity()](/cells/it/python-net/aspose.cells/metered/get_consumption_quantity/#) | Ottiene la dimensione del file di consumo|
| [get_consumption_credit()](/cells/it/python-net/aspose.cells/metered/get_consumption_credit/#) | Ottiene credito al consumo|



###  Esempio

In questo esempio, verrà effettuato un tentativo di impostare la chiave pubblica e privata misurata


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Guarda anche
* modulo [aspose.cells](..)
