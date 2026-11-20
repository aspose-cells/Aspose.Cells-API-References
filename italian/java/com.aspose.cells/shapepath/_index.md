---
title: "ShapePath"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un percorso di creazione costituito da una serie di linee e curve di movimento che, combinati, formeranno una forma geometrica."
type: docs
url: /it/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

Rappresenta un percorso di creazione costituito da una serie di spostamenti, linee e curve che, combinati, formeranno una forma geometrica.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ShapePath()](#ShapePath--) | Inizializza una nuova istanza della classe [ShapePath](../../com.aspose.cells/shapepath). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | Aggiunge un arco ellittico alla figura corrente. |
| [close()](#close--) | Chiude la figura corrente e avvia una nuova figura. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | Aggiunge una curva cubica B\u8305zier alla figura corrente. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Ottiene l'altezza di questo percorso in unità di pixel. |
| [getPathSegementList()](#getPathSegementList--) | Ottiene l'elenco [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getPathSegments()](#getPathSegments--) | Ottiene l'elenco [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getWidthPixel()](#getWidthPixel--) | Ottiene la larghezza di questo percorso in unità di pixel. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | Aggiunge un segmento di linea alla figura corrente. |
| [moveTo(float x, float y)](#moveTo-float-float-) | Avvia una nuova figura dal punto specificato senza chiudere la figura corrente. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Ottiene l'altezza di questo percorso in unità di pixel. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Ottiene la larghezza di questo percorso in unità di pixel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


Inizializza una nuova istanza della classe [ShapePath](../../com.aspose.cells/shapepath).

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


Aggiunge un arco ellittico alla figura corrente. Il punto di partenza è il punto finale della figura corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| wR | float | La metà della larghezza dell'area rettangolare dell'ellisse \\u9225\\u5b27\\u20ac\\u5aa1 che disegna l'arco (Unità: Pixel). |
| hR | float | La metà dell'altezza dell'area rettangolare dell'ellisse \\u9225\\u5b27\\u20ac\\u5aa1 che disegna l'arco (Unità: Pixel). |
| stAng | float | L'angolo di partenza dell'arco, misurato in gradi in senso orario dall'asse x (Unità: Grado). Questo angolo specificherà quale angolo lungo il percorso circolare previsto sarà usato come posizione iniziale per disegnare l'arco. Questo angolo di partenza sarà bloccato all'ultima posizione nota della penna nel percorso della forma, garantendo così un percorso di forma continuo. |
| swAng | float | L'angolo di oscillazione per un arco. Questo angolo specificherà fino a che punto, in termini di angolo, lungo il percorso circolare previsto l'arco sarà esteso. L'estensione dall'angolo di partenza sarà sempre in senso orario attorno al cerchio previsto. (Unità: Grado) |

### close() {#close--}
```
public void close()
```


Chiude la figura corrente e avvia una nuova figura. Se la figura corrente contiene una sequenza di linee e curve collegate, il metodo chiude il ciclo collegando una linea dal punto finale al punto di partenza.

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


Aggiunge una curva cubica B\\u8305zier alla figura corrente. Il punto di partenza è il punto finale della figura corrente. (Unità: Pixel).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ctrX1 | float | La coordinata x del primo punto di controllo della curva (Unità: Pixel). |
| ctrY1 | float | La coordinata y del primo punto di controllo della curva (Unità: Pixel). |
| ctrX2 | float | La coordinata x del secondo punto di controllo della curva (Unità: Pixel). |
| ctrY2 | float | La coordinata y del secondo punto di controllo della curva (Unità: Pixel). |
| endX | float | La coordinata x del punto finale della curva (Unità: Pixel). |
| endY | float | La coordinata y del punto finale della curva (Unità: Pixel). |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Ottiene l'altezza di questo percorso in unità di pixel.

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


Ottiene l'elenco [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ShapePath.PathSegments. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


Ottiene l'elenco [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Ottiene la larghezza di questo percorso in unità di pixel.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### lineTo(float x, float y) {#lineTo-float-float-}
```
public void lineTo(float x, float y)
```


Aggiunge un segmento di linea alla figura corrente. Il punto di partenza è il punto finale della figura corrente. (Unità: Pixel).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| x | float | La coordinata x del punto finale del segmento di linea(Unit: Pixel). |
| y | float | La coordinata y del punto finale del segmento di linea(Unit: Pixel). |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


Avvia una nuova figura dal punto specificato senza chiudere la figura corrente. Tutti i punti successivi aggiunti al percorso vengono aggiunti a questa nuova figura.Unit: Pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| x | float | La coordinata x del punto di partenza della figura(Unit: Pixel). |
| y | float | La coordinata y del punto di partenza della figura(Unit: Pixel). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Ottiene l'altezza di questo percorso in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Ottiene la larghezza di questo percorso in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

