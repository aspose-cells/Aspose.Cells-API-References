---
title: "ThreeDFormat"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la formattazione tridimensionale di una forma."
type: docs
url: /it/java/com.aspose.cells/threedformat/
---

**Inheritance:**
java.lang.Object
```
public class ThreeDFormat
```

Rappresenta la formattazione tridimensionale di una forma.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomBevelHeight()](#getBottomBevelHeight--) | Restituisce l'altezza del bordo inferiore, o quanto è applicato nella forma. |
| [getBottomBevelType()](#getBottomBevelType--) | Restituisce il tipo del bordo inferiore, o quanto è applicato nella forma. |
| [getBottomBevelWidth()](#getBottomBevelWidth--) | Restituisce la larghezza del bordo inferiore, o quanto è applicato nella forma. |
| [getClass()](#getClass--) |  |
| [getContourColor()](#getContourColor--) | Restituisce il colore del contorno su una forma. |
| [getContourWidth()](#getContourWidth--) | Restituisce la larghezza del contorno sulla forma, in unità di punti. |
| [getExtrusionColor()](#getExtrusionColor--) | Restituisce il colore dell'estrusione su una forma. |
| [getExtrusionHeight()](#getExtrusionHeight--) | Restituisce l'altezza dell'estrusione applicata alla forma, in unità di punti. |
| [getLightAngle()](#getLightAngle--) | Restituisce l'angolo delle luci di estrusione. |
| [getLighting()](#getLighting--) | Ottiene il tipo di impianto di luce. |
| [getLightingDirection()](#getLightingDirection--) | Ottiene la direzione da cui l'impianto di luce è orientato rispetto alla scena. |
| [getMaterial()](#getMaterial--) | Rappresenta il materiale predefinito che viene combinato con le proprietà di illuminazione per fornire l'aspetto finale di una forma. |
| [getPerspective()](#getPerspective--) | Ottiene l'angolo da cui un oggetto ThreeDFormat può essere visualizzato. |
| [getPresetCameraType()](#getPresetCameraType--) | Ottiene il tipo di telecamera predefinita per l'estrusione. |
| [getRotationX()](#getRotationX--) | Ottiene la rotazione della forma estrusa attorno all'asse x in gradi. |
| [getRotationY()](#getRotationY--) | Ottiene la rotazione della forma estrusa attorno all'asse y in gradi. |
| [getRotationZ()](#getRotationZ--) | Ottiene la rotazione della forma estrusa attorno all'asse z in gradi. |
| [getTopBevelHeight()](#getTopBevelHeight--) | Ottiene l'altezza del raccordo superiore, o quanto in profondità viene applicato alla forma. |
| [getTopBevelType()](#getTopBevelType--) | Ottiene il tipo di raccordo superiore, o quanto in profondità viene applicato alla forma. |
| [getTopBevelWidth()](#getTopBevelWidth--) | Ottiene la larghezza del raccordo superiore, o quanto in profondità viene applicato alla forma. |
| [getZ()](#getZ--) | Definisce la distanza dal suolo per la forma 3D. |
| [hashCode()](#hashCode--) | Ottiene il codice hash. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottomBevelHeight(double value)](#setBottomBevelHeight-double-) | Imposta l'altezza del raccordo inferiore, o quanto in profondità viene applicato alla forma. |
| [setBottomBevelType(int value)](#setBottomBevelType-int-) | Imposta il tipo di raccordo inferiore, o quanto in profondità viene applicato alla forma. |
| [setBottomBevelWidth(double value)](#setBottomBevelWidth-double-) | Imposta la larghezza del raccordo inferiore, o quanto in profondità viene applicato alla forma. |
| [setContourColor(CellsColor value)](#setContourColor-com.aspose.cells.CellsColor-) | Imposta il colore del contorno su una forma. |
| [setContourWidth(double value)](#setContourWidth-double-) | Imposta la larghezza del contorno sulla forma, in unità di punti. |
| [setExtrusionColor(CellsColor value)](#setExtrusionColor-com.aspose.cells.CellsColor-) | Restituisce il colore dell'estrusione su una forma. |
| [setExtrusionHeight(double value)](#setExtrusionHeight-double-) | Imposta l'altezza di estrusione applicata alla forma, in unità di punti. |
| [setLightAngle(double value)](#setLightAngle-double-) | Imposta l'angolo delle luci di estrusione. |
| [setLighting(int value)](#setLighting-int-) | Imposta il tipo di impianto di luce. |
| [setLightingDirection(int value)](#setLightingDirection-int-) | Imposta la direzione da cui l'impianto di luce è orientato rispetto alla scena. |
| [setMaterial(int value)](#setMaterial-int-) | Rappresenta il materiale predefinito che viene combinato con le proprietà di illuminazione per fornire l'aspetto finale di una forma. |
| [setPerspective(double value)](#setPerspective-double-) | Imposta l'angolo da cui un oggetto ThreeDFormat può essere visualizzato. |
| [setPresetCameraType(int value)](#setPresetCameraType-int-) | Imposta il tipo di telecamera predefinita per l'estrusione. |
| [setRotationX(double value)](#setRotationX-double-) | Imposta la rotazione della forma estrusa attorno all'asse x in gradi. |
| [setRotationY(double value)](#setRotationY-double-) | Imposta la rotazione della forma estrusa attorno all'asse y in gradi. |
| [setRotationZ(double value)](#setRotationZ-double-) | Imposta la rotazione della forma estrusa attorno all'asse z in gradi. |
| [setTopBevelHeight(double value)](#setTopBevelHeight-double-) | Imposta l'altezza dello smusso superiore, o quanto in profondità nella forma viene applicato. |
| [setTopBevelType(int value)](#setTopBevelType-int-) | Imposta il tipo dello smusso superiore, o quanto in profondità nella forma viene applicato. |
| [setTopBevelWidth(double value)](#setTopBevelWidth-double-) | Imposta la larghezza dello smusso superiore, o quanto in profondità nella forma viene applicato. |
| [setZ(double value)](#setZ-double-) | Definisce la distanza dal suolo per la forma 3D. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomBevelHeight() {#getBottomBevelHeight--}
```
public double getBottomBevelHeight()
```


Restituisce l'altezza dello smusso inferiore, o quanto in profondità nella forma viene applicato. In unità di punti.

**Returns:**
double
### getBottomBevelType() {#getBottomBevelType--}
```
public int getBottomBevelType()
```


Restituisce il tipo dello smusso inferiore, o quanto in profondità nella forma viene applicato. In unità di punti.

Vedi [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getBottomBevelWidth() {#getBottomBevelWidth--}
```
public double getBottomBevelWidth()
```


Restituisce la larghezza dello smusso inferiore, o quanto in profondità nella forma viene applicato. In unità di punti.

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getContourColor() {#getContourColor--}
```
public CellsColor getContourColor()
```


Restituisce il colore del contorno su una forma.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getContourWidth() {#getContourWidth--}
```
public double getContourWidth()
```


Restituisce la larghezza del contorno sulla forma, in unità di punti.

**Returns:**
double
### getExtrusionColor() {#getExtrusionColor--}
```
public CellsColor getExtrusionColor()
```


Restituisce il colore dell'estrusione su una forma.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getExtrusionHeight() {#getExtrusionHeight--}
```
public double getExtrusionHeight()
```


Restituisce l'altezza dell'estrusione applicata alla forma, in unità di punti.

**Returns:**
double
### getLightAngle() {#getLightAngle--}
```
public double getLightAngle()
```


Restituisce l'angolo delle luci di estrusione.

**Returns:**
double
### getLighting() {#getLighting--}
```
public int getLighting()
```


Ottiene il tipo di impianto di luce.

Vedi [LightRigType](../../com.aspose.cells/lightrigtype).

**Returns:**
int
### getLightingDirection() {#getLightingDirection--}
```
public int getLightingDirection()
```


Ottiene la direzione da cui l'impianto di luce è orientato rispetto alla scena.

Vedi [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Returns:**
int
### getMaterial() {#getMaterial--}
```
public int getMaterial()
```


Rappresenta il materiale predefinito che viene combinato con le proprietà di illuminazione per fornire l'aspetto finale di una forma.

Vedi [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Returns:**
int
### getPerspective() {#getPerspective--}
```
public double getPerspective()
```


Ottiene l'angolo da cui un oggetto ThreeDFormat può essere visualizzato.

**Returns:**
double
### getPresetCameraType() {#getPresetCameraType--}
```
public int getPresetCameraType()
```


Ottiene il tipo di telecamera predefinita per l'estrusione.

Vedi [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Returns:**
int
### getRotationX() {#getRotationX--}
```
public double getRotationX()
```


Ottiene la rotazione della forma estrusa attorno all'asse x in gradi.

**Returns:**
double
### getRotationY() {#getRotationY--}
```
public double getRotationY()
```


Ottiene la rotazione della forma estrusa attorno all'asse y in gradi.

**Returns:**
double
### getRotationZ() {#getRotationZ--}
```
public double getRotationZ()
```


Ottiene la rotazione della forma estrusa attorno all'asse z in gradi.

**Returns:**
double
### getTopBevelHeight() {#getTopBevelHeight--}
```
public double getTopBevelHeight()
```


Restituisce l'altezza dello smusso superiore, o quanto in profondità nella forma viene applicato. In unità di punti.

**Returns:**
double
### getTopBevelType() {#getTopBevelType--}
```
public int getTopBevelType()
```


Restituisce il tipo dello smusso superiore, o quanto in profondità nella forma viene applicato. In unità di punti.

Vedi [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getTopBevelWidth() {#getTopBevelWidth--}
```
public double getTopBevelWidth()
```


Restituisce la larghezza dello smusso superiore, o quanto in profondità nella forma viene applicato. In unità di punti.

**Returns:**
double
### getZ() {#getZ--}
```
public double getZ()
```


Definisce la distanza dal suolo per la forma 3D.

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


Ottiene il codice hash.

**Returns:**
int -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBottomBevelHeight(double value) {#setBottomBevelHeight-double-}
```
public void setBottomBevelHeight(double value)
```


Imposta l'altezza dello smusso inferiore, o quanto in profondità nella forma viene applicato. In unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setBottomBevelType(int value) {#setBottomBevelType-int-}
```
public void setBottomBevelType(int value)
```


Imposta il tipo dello smusso inferiore, o quanto in profondità nella forma viene applicato. In unità di punti.

Vedi [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBottomBevelWidth(double value) {#setBottomBevelWidth-double-}
```
public void setBottomBevelWidth(double value)
```


Imposta la larghezza dello smusso inferiore, o quanto in profondità nella forma viene applicato. In unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setContourColor(CellsColor value) {#setContourColor-com.aspose.cells.CellsColor-}
```
public void setContourColor(CellsColor value)
```


Imposta il colore del contorno su una forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setContourWidth(double value) {#setContourWidth-double-}
```
public void setContourWidth(double value)
```


Imposta la larghezza del contorno sulla forma, in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setExtrusionColor(CellsColor value) {#setExtrusionColor-com.aspose.cells.CellsColor-}
```
public void setExtrusionColor(CellsColor value)
```


Restituisce il colore dell'estrusione su una forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setExtrusionHeight(double value) {#setExtrusionHeight-double-}
```
public void setExtrusionHeight(double value)
```


Imposta l'altezza di estrusione applicata alla forma, in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLightAngle(double value) {#setLightAngle-double-}
```
public void setLightAngle(double value)
```


Imposta l'angolo delle luci di estrusione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLighting(int value) {#setLighting-int-}
```
public void setLighting(int value)
```


Imposta il tipo di impianto di luce.

Vedi [LightRigType](../../com.aspose.cells/lightrigtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLightingDirection(int value) {#setLightingDirection-int-}
```
public void setLightingDirection(int value)
```


Imposta la direzione da cui l'impianto di luce è orientato rispetto alla scena.

Vedi [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaterial(int value) {#setMaterial-int-}
```
public void setMaterial(int value)
```


Rappresenta il materiale predefinito che viene combinato con le proprietà di illuminazione per fornire l'aspetto finale di una forma.

Vedi [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPerspective(double value) {#setPerspective-double-}
```
public void setPerspective(double value)
```


Imposta l'angolo da cui un oggetto ThreeDFormat può essere visualizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setPresetCameraType(int value) {#setPresetCameraType-int-}
```
public void setPresetCameraType(int value)
```


Imposta il tipo di telecamera predefinita per l'estrusione.

Vedi [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRotationX(double value) {#setRotationX-double-}
```
public void setRotationX(double value)
```


Imposta la rotazione della forma estrusa attorno all'asse x in gradi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setRotationY(double value) {#setRotationY-double-}
```
public void setRotationY(double value)
```


Imposta la rotazione della forma estrusa attorno all'asse y in gradi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setRotationZ(double value) {#setRotationZ-double-}
```
public void setRotationZ(double value)
```


Imposta la rotazione della forma estrusa attorno all'asse z in gradi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTopBevelHeight(double value) {#setTopBevelHeight-double-}
```
public void setTopBevelHeight(double value)
```


Imposta l'altezza dello smusso superiore, o quanto in profondità nella forma viene applicato. In unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTopBevelType(int value) {#setTopBevelType-int-}
```
public void setTopBevelType(int value)
```


Imposta il tipo dello smusso superiore, o quanto in profondità nella forma viene applicato. In unità di punti.

Vedi [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTopBevelWidth(double value) {#setTopBevelWidth-double-}
```
public void setTopBevelWidth(double value)
```


Imposta la larghezza dello smusso superiore, o quanto in profondità nella forma viene applicato. In unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setZ(double value) {#setZ-double-}
```
public void setZ(double value)
```


Definisce la distanza dal suolo per la forma 3D.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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

