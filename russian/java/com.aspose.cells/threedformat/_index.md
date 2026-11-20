---
title: "ThreeDFormat"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет трехмерное форматирование фигур."
type: docs
url: /ru/java/com.aspose.cells/threedformat/
---

**Inheritance:**
java.lang.Object
```
public class ThreeDFormat
```

Представляет трёхмерное форматирование фигуры.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomBevelHeight()](#getBottomBevelHeight--) | Получает высоту нижнего фаски или насколько глубоко она применяется к фигуре. |
| [getBottomBevelType()](#getBottomBevelType--) | Получает тип нижней фаски или насколько глубоко она применяется к фигуре. |
| [getBottomBevelWidth()](#getBottomBevelWidth--) | Получает ширину нижней фаски или насколько глубоко она применяется к фигуре. |
| [getClass()](#getClass--) |  |
| [getContourColor()](#getContourColor--) | Получает цвет контура фигуры. |
| [getContourWidth()](#getContourWidth--) | Получает ширину контура фигуры в пунктах. |
| [getExtrusionColor()](#getExtrusionColor--) | Получает цвет выдавливания фигуры. |
| [getExtrusionHeight()](#getExtrusionHeight--) | Получает высоту выдавливания, применяемую к фигуре, в пунктах. |
| [getLightAngle()](#getLightAngle--) | Получает угол света выдавливания. |
| [getLighting()](#getLighting--) | Получает тип световой установки. |
| [getLightingDirection()](#getLightingDirection--) | Получает направление, из которого световая установка ориентирована относительно сцены. |
| [getMaterial()](#getMaterial--) | Представляет предустановленный материал, который комбинируется со свойствами освещения, чтобы придать окончательный вид и ощущение форме. |
| [getPerspective()](#getPerspective--) | Получает угол, под которым можно просматривать объект ThreeDFormat. |
| [getPresetCameraType()](#getPresetCameraType--) | Получает тип предустановленной камеры экструдирования. |
| [getRotationX()](#getRotationX--) | Получает вращение экструдированной формы вокруг оси X в градусах. |
| [getRotationY()](#getRotationY--) | Получает вращение экструдированной формы вокруг оси Y в градусах. |
| [getRotationZ()](#getRotationZ--) | Получает вращение экструдированной формы вокруг оси Z в градусах. |
| [getTopBevelHeight()](#getTopBevelHeight--) | Получает высоту верхней фаски, или насколько глубоко она применяется к форме. |
| [getTopBevelType()](#getTopBevelType--) | Получает тип верхней фаски, или насколько глубоко она применяется к форме. |
| [getTopBevelWidth()](#getTopBevelWidth--) | Получает ширину верхней фаски, или насколько глубоко она применяется к форме. |
| [getZ()](#getZ--) | Определяет расстояние от земли для 3D‑формы. |
| [hashCode()](#hashCode--) | Получает хеш-код. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottomBevelHeight(double value)](#setBottomBevelHeight-double-) | Устанавливает высоту нижней фаски, или насколько глубоко она применяется к форме. |
| [setBottomBevelType(int value)](#setBottomBevelType-int-) | Устанавливает тип нижней фаски, или насколько глубоко она применяется к форме. |
| [setBottomBevelWidth(double value)](#setBottomBevelWidth-double-) | Устанавливает ширину нижней фаски, или насколько глубоко она применяется к форме. |
| [setContourColor(CellsColor value)](#setContourColor-com.aspose.cells.CellsColor-) | Устанавливает цвет контура на форме. |
| [setContourWidth(double value)](#setContourWidth-double-) | Устанавливает ширину контура на форме, в единицах пунктов. |
| [setExtrusionColor(CellsColor value)](#setExtrusionColor-com.aspose.cells.CellsColor-) | Получает цвет выдавливания фигуры. |
| [setExtrusionHeight(double value)](#setExtrusionHeight-double-) | Устанавливает высоту экструдирования, применяемую к форме, в единицах пунктов. |
| [setLightAngle(double value)](#setLightAngle-double-) | Устанавливает угол света экструдирования. |
| [setLighting(int value)](#setLighting-int-) | Устанавливает тип световой установки. |
| [setLightingDirection(int value)](#setLightingDirection-int-) | Устанавливает направление, из которого световая установка ориентирована относительно сцены. |
| [setMaterial(int value)](#setMaterial-int-) | Представляет предустановленный материал, который комбинируется со свойствами освещения, чтобы придать окончательный вид и ощущение форме. |
| [setPerspective(double value)](#setPerspective-double-) | Устанавливает угол, под которым можно просматривать объект ThreeDFormat. |
| [setPresetCameraType(int value)](#setPresetCameraType-int-) | Устанавливает тип предустановленной камеры экструдирования. |
| [setRotationX(double value)](#setRotationX-double-) | Устанавливает вращение экструдированной формы вокруг оси X в градусах. |
| [setRotationY(double value)](#setRotationY-double-) | Устанавливает вращение выдавленной формы вокруг оси y в градусах. |
| [setRotationZ(double value)](#setRotationZ-double-) | Устанавливает вращение выдавленной формы вокруг оси z в градусах. |
| [setTopBevelHeight(double value)](#setTopBevelHeight-double-) | Устанавливает высоту верхней фаски или насколько глубоко она применяется к форме. |
| [setTopBevelType(int value)](#setTopBevelType-int-) | Устанавливает тип верхней фаски или насколько глубоко она применяется к форме. |
| [setTopBevelWidth(double value)](#setTopBevelWidth-double-) | Устанавливает ширину верхней фаски или насколько глубоко она применяется к форме. |
| [setZ(double value)](#setZ-double-) | Определяет расстояние от земли для 3D‑формы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomBevelHeight() {#getBottomBevelHeight--}
```
public double getBottomBevelHeight()
```


Получает высоту нижней фаски или насколько глубоко она применяется к форме. В единицах точек.

**Returns:**
double
### getBottomBevelType() {#getBottomBevelType--}
```
public int getBottomBevelType()
```


Получает тип нижней фаски или насколько глубоко она применяется к форме. В единицах точек.

См. [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getBottomBevelWidth() {#getBottomBevelWidth--}
```
public double getBottomBevelWidth()
```


Получает ширину нижней фаски или насколько глубоко она применяется к форме. В единицах точек.

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


Получает цвет контура фигуры.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getContourWidth() {#getContourWidth--}
```
public double getContourWidth()
```


Получает ширину контура фигуры в пунктах.

**Returns:**
double
### getExtrusionColor() {#getExtrusionColor--}
```
public CellsColor getExtrusionColor()
```


Получает цвет выдавливания фигуры.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getExtrusionHeight() {#getExtrusionHeight--}
```
public double getExtrusionHeight()
```


Получает высоту выдавливания, применяемую к фигуре, в пунктах.

**Returns:**
double
### getLightAngle() {#getLightAngle--}
```
public double getLightAngle()
```


Получает угол света выдавливания.

**Returns:**
double
### getLighting() {#getLighting--}
```
public int getLighting()
```


Получает тип световой установки.

См. [LightRigType](../../com.aspose.cells/lightrigtype).

**Returns:**
int
### getLightingDirection() {#getLightingDirection--}
```
public int getLightingDirection()
```


Получает направление, из которого световая установка ориентирована относительно сцены.

См. [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Returns:**
int
### getMaterial() {#getMaterial--}
```
public int getMaterial()
```


Представляет предустановленный материал, который комбинируется со свойствами освещения, чтобы придать окончательный вид и ощущение форме.

См. [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Returns:**
int
### getPerspective() {#getPerspective--}
```
public double getPerspective()
```


Получает угол, под которым можно просматривать объект ThreeDFormat.

**Returns:**
double
### getPresetCameraType() {#getPresetCameraType--}
```
public int getPresetCameraType()
```


Получает тип предустановленной камеры экструдирования.

См. [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Returns:**
int
### getRotationX() {#getRotationX--}
```
public double getRotationX()
```


Получает вращение экструдированной формы вокруг оси X в градусах.

**Returns:**
double
### getRotationY() {#getRotationY--}
```
public double getRotationY()
```


Получает вращение экструдированной формы вокруг оси Y в градусах.

**Returns:**
double
### getRotationZ() {#getRotationZ--}
```
public double getRotationZ()
```


Получает вращение экструдированной формы вокруг оси Z в градусах.

**Returns:**
double
### getTopBevelHeight() {#getTopBevelHeight--}
```
public double getTopBevelHeight()
```


Получает высоту верхней фаски или насколько глубоко она применяется к форме. В единицах точек.

**Returns:**
double
### getTopBevelType() {#getTopBevelType--}
```
public int getTopBevelType()
```


Получает тип верхней фаски или насколько глубоко она применяется к форме. В единицах точек.

См. [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getTopBevelWidth() {#getTopBevelWidth--}
```
public double getTopBevelWidth()
```


Получает ширину верхней фаски или насколько глубоко она применяется к форме. В единицах точек.

**Returns:**
double
### getZ() {#getZ--}
```
public double getZ()
```


Определяет расстояние от земли для 3D‑формы.

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


Получает хеш-код.

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


Устанавливает высоту нижней фаски или насколько глубоко она применяется к форме. В единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setBottomBevelType(int value) {#setBottomBevelType-int-}
```
public void setBottomBevelType(int value)
```


Устанавливает тип нижней фаски или насколько глубоко она применяется к форме. В единицах точек.

См. [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBottomBevelWidth(double value) {#setBottomBevelWidth-double-}
```
public void setBottomBevelWidth(double value)
```


Устанавливает ширину нижней фаски или насколько глубоко она применяется к форме. В единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setContourColor(CellsColor value) {#setContourColor-com.aspose.cells.CellsColor-}
```
public void setContourColor(CellsColor value)
```


Устанавливает цвет контура на форме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setContourWidth(double value) {#setContourWidth-double-}
```
public void setContourWidth(double value)
```


Устанавливает ширину контура на форме, в единицах пунктов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setExtrusionColor(CellsColor value) {#setExtrusionColor-com.aspose.cells.CellsColor-}
```
public void setExtrusionColor(CellsColor value)
```


Получает цвет выдавливания фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setExtrusionHeight(double value) {#setExtrusionHeight-double-}
```
public void setExtrusionHeight(double value)
```


Устанавливает высоту экструдирования, применяемую к форме, в единицах пунктов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLightAngle(double value) {#setLightAngle-double-}
```
public void setLightAngle(double value)
```


Устанавливает угол света экструдирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLighting(int value) {#setLighting-int-}
```
public void setLighting(int value)
```


Устанавливает тип световой установки.

См. [LightRigType](../../com.aspose.cells/lightrigtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLightingDirection(int value) {#setLightingDirection-int-}
```
public void setLightingDirection(int value)
```


Устанавливает направление, из которого световая установка ориентирована относительно сцены.

См. [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaterial(int value) {#setMaterial-int-}
```
public void setMaterial(int value)
```


Представляет предустановленный материал, который комбинируется со свойствами освещения, чтобы придать окончательный вид и ощущение форме.

См. [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPerspective(double value) {#setPerspective-double-}
```
public void setPerspective(double value)
```


Устанавливает угол, под которым можно просматривать объект ThreeDFormat.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setPresetCameraType(int value) {#setPresetCameraType-int-}
```
public void setPresetCameraType(int value)
```


Устанавливает тип предустановленной камеры экструдирования.

См. [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRotationX(double value) {#setRotationX-double-}
```
public void setRotationX(double value)
```


Устанавливает вращение экструдированной формы вокруг оси X в градусах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setRotationY(double value) {#setRotationY-double-}
```
public void setRotationY(double value)
```


Устанавливает вращение выдавленной формы вокруг оси y в градусах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setRotationZ(double value) {#setRotationZ-double-}
```
public void setRotationZ(double value)
```


Устанавливает вращение выдавленной формы вокруг оси z в градусах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTopBevelHeight(double value) {#setTopBevelHeight-double-}
```
public void setTopBevelHeight(double value)
```


Устанавливает высоту верхней фаски или насколько глубоко она применяется к форме. В единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTopBevelType(int value) {#setTopBevelType-int-}
```
public void setTopBevelType(int value)
```


Устанавливает тип верхней фаски или насколько глубоко она применяется к форме. В единицах точек.

См. [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTopBevelWidth(double value) {#setTopBevelWidth-double-}
```
public void setTopBevelWidth(double value)
```


Устанавливает ширину верхней фаски или насколько глубоко она применяется к форме. В единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setZ(double value) {#setZ-double-}
```
public void setZ(double value)
```


Определяет расстояние от земли для 3D‑формы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

