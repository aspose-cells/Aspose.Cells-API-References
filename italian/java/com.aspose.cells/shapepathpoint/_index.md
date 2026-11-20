---
title: "ShapePathPoint"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Specifica le coordinate di posizione o i marcatori di angolo."
type: docs
url: /it/java/com.aspose.cells/shapepathpoint/
---

**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```

Specifica le coordinate di posizione o i marcatori di angolo. Le coordinate di posizione rappresentano le coordinate di un percorso in uno spazio di coordinate (ad es. X/Y). I marcatori di angolo indicano le variazioni angolari in un percorso (ad es. gli angoli di inizio e di swing di un arco).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Specifica il tipo di valore dell'oggetto corrente. |
| [getX()](#getX--) | Restituisce la coordinata x per questa coordinata di posizione. |
| [getXAngle()](#getXAngle--) | Quando l'oggetto è un marcatore di angolo, ottieni o imposta il primo angolo in gradi. |
| [getXPixel()](#getXPixel--) | Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata x in pixel. |
| [getY()](#getY--) | Restituisce la coordinata y per questa coordinata di posizione. |
| [getYAngle()](#getYAngle--) | Quando l'oggetto è un marcatore di angolo, ottieni o imposta il secondo angolo in gradi. |
| [getYPixel()](#getYPixel--) | Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata y in pixel. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | Imposta la coordinata x per questa coordinata di posizione. |
| [setXAngle(int value)](#setXAngle-int-) | Quando l'oggetto è un marcatore di angolo, ottieni o imposta il primo angolo in gradi. |
| [setXPixel(int value)](#setXPixel-int-) | Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata x in pixel. |
| [setY(int value)](#setY-int-) | Restituisce la coordinata y per questa coordinata di posizione. |
| [setYAngle(int value)](#setYAngle-int-) | Quando l'oggetto è un marcatore di angolo, ottieni o imposta il secondo angolo in gradi. |
| [setYPixel(int value)](#setYPixel-int-) | Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata y in pixel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getType() {#getType--}
```
public int getType()
```


Specifica il tipo di valore dell'oggetto corrente.

Vedi [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype).

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Restituisce la coordinata x per questa coordinata di posizione. Unità EMU.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare le proprietà ShapePathPoint.XPixel e ShapePathPoint.XAngle. Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```


Quando l'oggetto è un marcatore di angolo, ottieni o imposta il primo angolo in gradi.

**Remarks**

Se questo angolo è l'angolo iniziale di un arco. Questo angolo specificherà quale angolo lungo il percorso circolare presunto verrà utilizzato come posizione di partenza per disegnare l'arco. Questo angolo di partenza sarà bloccato all'ultima posizione nota della penna nel percorso della forma. Garantendo così un percorso della forma continuo.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata x in pixel.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Restituisce la coordinata y per questa coordinata di posizione. Unità EMU.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare le proprietà ShapePathPoint.YPixel e ShapePathPoint.YAngle. Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```


Quando l'oggetto è un marcatore di angolo, ottieni o imposta il secondo angolo in gradi.

**Remarks**

Se questo angolo è l'angolo di oscillazione di un arco. Questo angolo specificherà quanto lontano, in termini di angolo, lungo il percorso circolare presunto l'arco sarà esteso. L'estensione dall'angolo di partenza sarà sempre nella direzione oraria intorno al cerchio presunto.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata y in pixel.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Imposta la coordinata x per questa coordinata di posizione. Unità EMU.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare le proprietà ShapePathPoint.XPixel e ShapePathPoint.XAngle. Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```


Quando l'oggetto è un marcatore di angolo, ottieni o imposta il primo angolo in gradi.

**Remarks**

Se questo angolo è l'angolo iniziale di un arco. Questo angolo specificherà quale angolo lungo il percorso circolare presunto verrà utilizzato come posizione di partenza per disegnare l'arco. Questo angolo di partenza sarà bloccato all'ultima posizione nota della penna nel percorso della forma. Garantendo così un percorso della forma continuo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata x in pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Restituisce la coordinata y per questa coordinata di posizione. Unità EMU.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare le proprietà ShapePathPoint.YPixel e ShapePathPoint.YAngle. Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```


Quando l'oggetto è un marcatore di angolo, ottieni o imposta il secondo angolo in gradi.

**Remarks**

Se questo angolo è l'angolo di oscillazione di un arco. Questo angolo specificherà quanto lontano, in termini di angolo, lungo il percorso circolare presunto l'arco sarà esteso. L'estensione dall'angolo di partenza sarà sempre nella direzione oraria intorno al cerchio presunto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Quando l'oggetto è una coordinata di posizione, ottieni o imposta la coordinata y in pixel.

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

