---
title: "ThreeDFormat"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en formes tredimensionella formatering."
type: docs
url: /sv/java/com.aspose.cells/threedformat/
---

**Inheritance:**
java.lang.Object
```
public class ThreeDFormat
```

Representerar en formens tredimensionella formatering.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomBevelHeight()](#getBottomBevelHeight--) | Hämtar höjden på den nedre fasen, eller hur långt in i formen den tillämpas. |
| [getBottomBevelType()](#getBottomBevelType--) | Hämtar typen av den nedre fasen, eller hur långt in i formen den tillämpas. |
| [getBottomBevelWidth()](#getBottomBevelWidth--) | Hämtar bredden på den nedre fasen, eller hur långt in i formen den tillämpas. |
| [getClass()](#getClass--) |  |
| [getContourColor()](#getContourColor--) | Hämtar konturfärgen på en form. |
| [getContourWidth()](#getContourWidth--) | Hämtar konturbredden på formen, i enheten punkter. |
| [getExtrusionColor()](#getExtrusionColor--) | Hämtar extruderingsfärgen på en form. |
| [getExtrusionHeight()](#getExtrusionHeight--) | Hämtar extruderingshöjden som tillämpas på formen, i enheten punkter. |
| [getLightAngle()](#getLightAngle--) | Hämtar vinkeln på extruderingsljusen. |
| [getLighting()](#getLighting--) | Hämtar typen av ljusrigg. |
| [getLightingDirection()](#getLightingDirection--) | Hämtar riktningen från vilken ljusriggen är orienterad i förhållande till scenen. |
| [getMaterial()](#getMaterial--) | Representerar det förinställda materialet som kombineras med ljusegenskaperna för att ge den slutliga utseendet och känslan av en form. |
| [getPerspective()](#getPerspective--) | Hämtar vinkeln där ett ThreeDFormat-objekt kan ses. |
| [getPresetCameraType()](#getPresetCameraType--) | Hämtar den förinställda kameratypen för extrudering. |
| [getRotationX()](#getRotationX--) | Hämtar rotationen av den extruderade formen runt x-axeln i grader. |
| [getRotationY()](#getRotationY--) | Hämtar rotationen av den extruderade formen runt y-axeln i grader. |
| [getRotationZ()](#getRotationZ--) | Hämtar rotationen av den extruderade formen runt z-axeln i grader. |
| [getTopBevelHeight()](#getTopBevelHeight--) | Hämtar höjden på den övre fasen, eller hur långt in i formen den tillämpas. |
| [getTopBevelType()](#getTopBevelType--) | Hämtar typen av den övre avfasningen, eller hur långt in i formen den tillämpas. |
| [getTopBevelWidth()](#getTopBevelWidth--) | Hämtar bredden på den övre avfasningen, eller hur långt in i formen den tillämpas. |
| [getZ()](#getZ--) | Definierar avståndet från marken för den 3D-formen. |
| [hashCode()](#hashCode--) | Hämtar hashkod. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottomBevelHeight(double value)](#setBottomBevelHeight-double-) | Ställer in höjden på den nedre avfasningen, eller hur långt in i formen den tillämpas. |
| [setBottomBevelType(int value)](#setBottomBevelType-int-) | Ställer in typen av den nedre avfasningen, eller hur långt in i formen den tillämpas. |
| [setBottomBevelWidth(double value)](#setBottomBevelWidth-double-) | Ställer in bredden på den nedre avfasningen, eller hur långt in i formen den tillämpas. |
| [setContourColor(CellsColor value)](#setContourColor-com.aspose.cells.CellsColor-) | Ställer in konturfärgen på en form. |
| [setContourWidth(double value)](#setContourWidth-double-) | Ställer in konturbredden på formen, i enheten punkter. |
| [setExtrusionColor(CellsColor value)](#setExtrusionColor-com.aspose.cells.CellsColor-) | Hämtar extruderingsfärgen på en form. |
| [setExtrusionHeight(double value)](#setExtrusionHeight-double-) | Ställer in extruderingshöjden som tillämpas på formen, i enheten punkter. |
| [setLightAngle(double value)](#setLightAngle-double-) | Ställer in vinkeln för extruderingsljusen. |
| [setLighting(int value)](#setLighting-int-) | Ställer in typ av ljusrigg. |
| [setLightingDirection(int value)](#setLightingDirection-int-) | Ställer in riktningen från vilken ljusriggen är orienterad i förhållande till scenen. |
| [setMaterial(int value)](#setMaterial-int-) | Representerar det förinställda materialet som kombineras med ljusegenskaperna för att ge den slutliga utseendet och känslan av en form. |
| [setPerspective(double value)](#setPerspective-double-) | Ställer in vinkeln där ett ThreeDFormat-objekt kan ses. |
| [setPresetCameraType(int value)](#setPresetCameraType-int-) | Ställer in den förinställda kameratypen för extrudering. |
| [setRotationX(double value)](#setRotationX-double-) | Ställer in rotationen av den extruderade formen kring x-axeln i grader. |
| [setRotationY(double value)](#setRotationY-double-) | Ställer in rotationen av den extruderade formen kring y-axeln i grader. |
| [setRotationZ(double value)](#setRotationZ-double-) | Ställer in rotationen av den extruderade formen kring z-axeln i grader. |
| [setTopBevelHeight(double value)](#setTopBevelHeight-double-) | Ställer in höjden på den övre avfasningen, eller hur långt in i formen den tillämpas. |
| [setTopBevelType(int value)](#setTopBevelType-int-) | Ställer in typen av den övre avfasningen, eller hur långt in i formen den tillämpas. |
| [setTopBevelWidth(double value)](#setTopBevelWidth-double-) | Ställer in bredden på den övre avfasningen, eller hur långt in i formen den tillämpas. |
| [setZ(double value)](#setZ-double-) | Definierar avståndet från marken för den 3D-formen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomBevelHeight() {#getBottomBevelHeight--}
```
public double getBottomBevelHeight()
```


Hämtar höjden på den nedre avfasningen, eller hur långt in i formen den tillämpas. I enheten punkter.

**Returns:**
double
### getBottomBevelType() {#getBottomBevelType--}
```
public int getBottomBevelType()
```


Hämtar typen av den nedre avfasningen, eller hur långt in i formen den tillämpas. I enheten punkter.

Se [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getBottomBevelWidth() {#getBottomBevelWidth--}
```
public double getBottomBevelWidth()
```


Hämtar bredden på den nedre avfasningen, eller hur långt in i formen den tillämpas. I enheten punkter.

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


Hämtar konturfärgen på en form.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getContourWidth() {#getContourWidth--}
```
public double getContourWidth()
```


Hämtar konturbredden på formen, i enheten punkter.

**Returns:**
double
### getExtrusionColor() {#getExtrusionColor--}
```
public CellsColor getExtrusionColor()
```


Hämtar extruderingsfärgen på en form.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getExtrusionHeight() {#getExtrusionHeight--}
```
public double getExtrusionHeight()
```


Hämtar extruderingshöjden som tillämpas på formen, i enheten punkter.

**Returns:**
double
### getLightAngle() {#getLightAngle--}
```
public double getLightAngle()
```


Hämtar vinkeln på extruderingsljusen.

**Returns:**
double
### getLighting() {#getLighting--}
```
public int getLighting()
```


Hämtar typen av ljusrigg.

Se [LightRigType](../../com.aspose.cells/lightrigtype).

**Returns:**
int
### getLightingDirection() {#getLightingDirection--}
```
public int getLightingDirection()
```


Hämtar riktningen från vilken ljusriggen är orienterad i förhållande till scenen.

Se [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Returns:**
int
### getMaterial() {#getMaterial--}
```
public int getMaterial()
```


Representerar det förinställda materialet som kombineras med ljusegenskaperna för att ge den slutliga utseendet och känslan av en form.

Se [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Returns:**
int
### getPerspective() {#getPerspective--}
```
public double getPerspective()
```


Hämtar vinkeln där ett ThreeDFormat-objekt kan ses.

**Returns:**
double
### getPresetCameraType() {#getPresetCameraType--}
```
public int getPresetCameraType()
```


Hämtar den förinställda kameratypen för extrudering.

Se [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Returns:**
int
### getRotationX() {#getRotationX--}
```
public double getRotationX()
```


Hämtar rotationen av den extruderade formen runt x-axeln i grader.

**Returns:**
double
### getRotationY() {#getRotationY--}
```
public double getRotationY()
```


Hämtar rotationen av den extruderade formen runt y-axeln i grader.

**Returns:**
double
### getRotationZ() {#getRotationZ--}
```
public double getRotationZ()
```


Hämtar rotationen av den extruderade formen runt z-axeln i grader.

**Returns:**
double
### getTopBevelHeight() {#getTopBevelHeight--}
```
public double getTopBevelHeight()
```


Hämtar höjden på den övre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

**Returns:**
double
### getTopBevelType() {#getTopBevelType--}
```
public int getTopBevelType()
```


Hämtar typen av den övre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

Se [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getTopBevelWidth() {#getTopBevelWidth--}
```
public double getTopBevelWidth()
```


Hämtar bredden på den övre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

**Returns:**
double
### getZ() {#getZ--}
```
public double getZ()
```


Definierar avståndet från marken för den 3D-formen.

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


Hämtar hashkod.

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


Ställer in höjden på den nedre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setBottomBevelType(int value) {#setBottomBevelType-int-}
```
public void setBottomBevelType(int value)
```


Ställer in typen av den nedre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

Se [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBottomBevelWidth(double value) {#setBottomBevelWidth-double-}
```
public void setBottomBevelWidth(double value)
```


Ställer in bredden på den nedre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setContourColor(CellsColor value) {#setContourColor-com.aspose.cells.CellsColor-}
```
public void setContourColor(CellsColor value)
```


Ställer in konturfärgen på en form.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setContourWidth(double value) {#setContourWidth-double-}
```
public void setContourWidth(double value)
```


Ställer in konturbredden på formen, i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setExtrusionColor(CellsColor value) {#setExtrusionColor-com.aspose.cells.CellsColor-}
```
public void setExtrusionColor(CellsColor value)
```


Hämtar extruderingsfärgen på en form.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setExtrusionHeight(double value) {#setExtrusionHeight-double-}
```
public void setExtrusionHeight(double value)
```


Ställer in extruderingshöjden som tillämpas på formen, i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLightAngle(double value) {#setLightAngle-double-}
```
public void setLightAngle(double value)
```


Ställer in vinkeln för extruderingsljusen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setLighting(int value) {#setLighting-int-}
```
public void setLighting(int value)
```


Ställer in typ av ljusrigg.

Se [LightRigType](../../com.aspose.cells/lightrigtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLightingDirection(int value) {#setLightingDirection-int-}
```
public void setLightingDirection(int value)
```


Ställer in riktningen från vilken ljusriggen är orienterad i förhållande till scenen.

Se [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaterial(int value) {#setMaterial-int-}
```
public void setMaterial(int value)
```


Representerar det förinställda materialet som kombineras med ljusegenskaperna för att ge den slutliga utseendet och känslan av en form.

Se [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPerspective(double value) {#setPerspective-double-}
```
public void setPerspective(double value)
```


Ställer in vinkeln där ett ThreeDFormat-objekt kan ses.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setPresetCameraType(int value) {#setPresetCameraType-int-}
```
public void setPresetCameraType(int value)
```


Ställer in den förinställda kameratypen för extrudering.

Se [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRotationX(double value) {#setRotationX-double-}
```
public void setRotationX(double value)
```


Ställer in rotationen av den extruderade formen kring x-axeln i grader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setRotationY(double value) {#setRotationY-double-}
```
public void setRotationY(double value)
```


Ställer in rotationen av den extruderade formen kring y-axeln i grader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setRotationZ(double value) {#setRotationZ-double-}
```
public void setRotationZ(double value)
```


Ställer in rotationen av den extruderade formen kring z-axeln i grader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTopBevelHeight(double value) {#setTopBevelHeight-double-}
```
public void setTopBevelHeight(double value)
```


Ställer in höjden på den övre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTopBevelType(int value) {#setTopBevelType-int-}
```
public void setTopBevelType(int value)
```


Ställer in typen av den övre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

Se [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTopBevelWidth(double value) {#setTopBevelWidth-double-}
```
public void setTopBevelWidth(double value)
```


Ställer in bredden på den övre fasaden, eller hur långt in i formen den tillämpas. I enheten Points.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setZ(double value) {#setZ-double-}
```
public void setZ(double value)
```


Definierar avståndet från marken för den 3D-formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

