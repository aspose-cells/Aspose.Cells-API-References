---
title: "ThreeDFormat"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir şeklin üç boyutlu biçimlendirmesini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/threedformat/
---

**Inheritance:**
java.lang.Object
```
public class ThreeDFormat
```

Bir şeklin üç boyutlu biçimlendirmesini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomBevelHeight()](#getBottomBevelHeight--) | Alt köşebentinin yüksekliğini alır, ya da şekle ne kadar uygulandığını alır. |
| [getBottomBevelType()](#getBottomBevelType--) | Alt köşebentinin tipini alır, ya da şekle ne kadar uygulandığını alır. |
| [getBottomBevelWidth()](#getBottomBevelWidth--) | Alt köşebentinin genişliğini alır, ya da şekle ne kadar uygulandığını alır. |
| [getClass()](#getClass--) |  |
| [getContourColor()](#getContourColor--) | Bir şeklin kontur rengini alır. |
| [getContourWidth()](#getContourWidth--) | Şeklin kontur genişliğini, puan biriminde alır. |
| [getExtrusionColor()](#getExtrusionColor--) | Bir şeklin ekstrüzyon rengini alır. |
| [getExtrusionHeight()](#getExtrusionHeight--) | Şekle uygulanan ekstrüzyon yüksekliğini, puan biriminde alır. |
| [getLightAngle()](#getLightAngle--) | Ekstrüzyon ışıklarının açısını alır. |
| [getLighting()](#getLighting--) | Işık setinin tipini alır. |
| [getLightingDirection()](#getLightingDirection--) | Işık setinin sahneye göre yönlendirildiği yönü alır. |
| [getMaterial()](#getMaterial--) | Şeklin son görünüm ve hissini sağlamak için aydınlatma özellikleriyle birleştirilen ön ayar malzemeyi temsil eder. |
| [getPerspective()](#getPerspective--) | Bir ThreeDFormat nesnesinin görüntülenebileceği açıyı alır. |
| [getPresetCameraType()](#getPresetCameraType--) | Ekstrüzyon ön ayar kamera tipini alır. |
| [getRotationX()](#getRotationX--) | Ekstrüde edilmiş şeklin x ekseni etrafındaki dönüşünü derece cinsinden alır. |
| [getRotationY()](#getRotationY--) | Ekstrüde edilmiş şeklin y ekseni etrafındaki dönüşünü derece cinsinden alır. |
| [getRotationZ()](#getRotationZ--) | Ekstrüde edilmiş şeklin z ekseni etrafındaki dönüşünü derece cinsinden alır. |
| [getTopBevelHeight()](#getTopBevelHeight--) | Üst köşegenin yüksekliğini, yani şekle ne kadar derinlikte uygulandığını alır. |
| [getTopBevelType()](#getTopBevelType--) | Üst köşegenin tipini, yani şekle ne kadar derinlikte uygulandığını alır. |
| [getTopBevelWidth()](#getTopBevelWidth--) | Üst köşegenin genişliğini, yani şekle ne kadar derinlikte uygulandığını alır. |
| [getZ()](#getZ--) | 3D şekil için yerden mesafeyi tanımlar. |
| [hashCode()](#hashCode--) | Hash kodunu alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottomBevelHeight(double value)](#setBottomBevelHeight-double-) | Alt köşegenin yüksekliğini, yani şekle ne kadar derinlikte uygulanacağını ayarlar. |
| [setBottomBevelType(int value)](#setBottomBevelType-int-) | Alt köşegenin tipini, yani şekle ne kadar derinlikte uygulanacağını ayarlar. |
| [setBottomBevelWidth(double value)](#setBottomBevelWidth-double-) | Alt köşegenin genişliğini, yani şekle ne kadar derinlikte uygulanacağını ayarlar. |
| [setContourColor(CellsColor value)](#setContourColor-com.aspose.cells.CellsColor-) | Bir şeklin kontur rengini ayarlar. |
| [setContourWidth(double value)](#setContourWidth-double-) | Şeklin kontur genişliğini, nokta biriminde ayarlar. |
| [setExtrusionColor(CellsColor value)](#setExtrusionColor-com.aspose.cells.CellsColor-) | Bir şeklin ekstrüzyon rengini alır. |
| [setExtrusionHeight(double value)](#setExtrusionHeight-double-) | Şekle uygulanan ekstrüzyon yüksekliğini, nokta biriminde ayarlar. |
| [setLightAngle(double value)](#setLightAngle-double-) | Ekstrüzyon ışıklarının açısını ayarlar. |
| [setLighting(int value)](#setLighting-int-) | Işık setinin tipini ayarlar. |
| [setLightingDirection(int value)](#setLightingDirection-int-) | Işık setinin sahneye göre yönlendirildiği yönü ayarlar. |
| [setMaterial(int value)](#setMaterial-int-) | Şeklin son görünüm ve hissini sağlamak için aydınlatma özellikleriyle birleştirilen ön ayar malzemeyi temsil eder. |
| [setPerspective(double value)](#setPerspective-double-) | Bir ThreeDFormat nesnesinin görüntülenebileceği açıyı ayarlar. |
| [setPresetCameraType(int value)](#setPresetCameraType-int-) | Ekstrüzyon ön ayar kamera tipini ayarlar. |
| [setRotationX(double value)](#setRotationX-double-) | Ekstrüde edilmiş şeklin x ekseni etrafındaki dönüşünü derece cinsinden ayarlar. |
| [setRotationY(double value)](#setRotationY-double-) | Ekstrüde şeklin y-eksenindeki dönüşünü derece cinsinden ayarlar. |
| [setRotationZ(double value)](#setRotationZ-double-) | Ekstrüde şeklin z-eksenindeki dönüşünü derece cinsinden ayarlar. |
| [setTopBevelHeight(double value)](#setTopBevelHeight-double-) | Üst köşe eğiminin yüksekliğini, yani şekle ne kadar uygulandığını ayarlar. |
| [setTopBevelType(int value)](#setTopBevelType-int-) | Üst köşe eğiminin tipini, yani şekle ne kadar uygulandığını ayarlar. |
| [setTopBevelWidth(double value)](#setTopBevelWidth-double-) | Üst köşe eğiminin genişliğini, yani şekle ne kadar uygulandığını ayarlar. |
| [setZ(double value)](#setZ-double-) | 3D şekil için yerden mesafeyi tanımlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomBevelHeight() {#getBottomBevelHeight--}
```
public double getBottomBevelHeight()
```


Alt köşe eğiminin yüksekliğini, yani şekle ne kadar uygulandığını alır. Nokta biriminde.

**Returns:**
double
### getBottomBevelType() {#getBottomBevelType--}
```
public int getBottomBevelType()
```


Alt köşe eğiminin tipini, yani şekle ne kadar uygulandığını alır. Nokta biriminde.

Bakınız [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getBottomBevelWidth() {#getBottomBevelWidth--}
```
public double getBottomBevelWidth()
```


Alt köşe eğiminin genişliğini, yani şekle ne kadar uygulandığını alır. Nokta biriminde.

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


Bir şeklin kontur rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getContourWidth() {#getContourWidth--}
```
public double getContourWidth()
```


Şeklin kontur genişliğini, puan biriminde alır.

**Returns:**
double
### getExtrusionColor() {#getExtrusionColor--}
```
public CellsColor getExtrusionColor()
```


Bir şeklin ekstrüzyon rengini alır.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getExtrusionHeight() {#getExtrusionHeight--}
```
public double getExtrusionHeight()
```


Şekle uygulanan ekstrüzyon yüksekliğini, puan biriminde alır.

**Returns:**
double
### getLightAngle() {#getLightAngle--}
```
public double getLightAngle()
```


Ekstrüzyon ışıklarının açısını alır.

**Returns:**
double
### getLighting() {#getLighting--}
```
public int getLighting()
```


Işık setinin tipini alır.

Bkz [LightRigType](../../com.aspose.cells/lightrigtype).

**Returns:**
int
### getLightingDirection() {#getLightingDirection--}
```
public int getLightingDirection()
```


Işık setinin sahneye göre yönlendirildiği yönü alır.

Bakınız [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Returns:**
int
### getMaterial() {#getMaterial--}
```
public int getMaterial()
```


Şeklin son görünüm ve hissini sağlamak için aydınlatma özellikleriyle birleştirilen ön ayar malzemeyi temsil eder.

Bkz [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Returns:**
int
### getPerspective() {#getPerspective--}
```
public double getPerspective()
```


Bir ThreeDFormat nesnesinin görüntülenebileceği açıyı alır.

**Returns:**
double
### getPresetCameraType() {#getPresetCameraType--}
```
public int getPresetCameraType()
```


Ekstrüzyon ön ayar kamera tipini alır.

Bakınız [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Returns:**
int
### getRotationX() {#getRotationX--}
```
public double getRotationX()
```


Ekstrüde edilmiş şeklin x ekseni etrafındaki dönüşünü derece cinsinden alır.

**Returns:**
double
### getRotationY() {#getRotationY--}
```
public double getRotationY()
```


Ekstrüde edilmiş şeklin y ekseni etrafındaki dönüşünü derece cinsinden alır.

**Returns:**
double
### getRotationZ() {#getRotationZ--}
```
public double getRotationZ()
```


Ekstrüde edilmiş şeklin z ekseni etrafındaki dönüşünü derece cinsinden alır.

**Returns:**
double
### getTopBevelHeight() {#getTopBevelHeight--}
```
public double getTopBevelHeight()
```


Üst köşe eğiminin yüksekliğini, yani şekle ne kadar uygulandığını alır. Nokta biriminde.

**Returns:**
double
### getTopBevelType() {#getTopBevelType--}
```
public int getTopBevelType()
```


Üst köşe eğiminin tipini, yani şekle ne kadar uygulandığını alır. Nokta biriminde.

Bakınız [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getTopBevelWidth() {#getTopBevelWidth--}
```
public double getTopBevelWidth()
```


Üst köşe eğiminin genişliğini, yani şekle ne kadar uygulandığını alır. Nokta biriminde.

**Returns:**
double
### getZ() {#getZ--}
```
public double getZ()
```


3D şekil için yerden mesafeyi tanımlar.

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


Hash kodunu alır.

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


Alt köşe eğiminin yüksekliğini, yani şekle ne kadar uygulandığını ayarlar. Nokta biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setBottomBevelType(int value) {#setBottomBevelType-int-}
```
public void setBottomBevelType(int value)
```


Alt köşe eğiminin tipini, yani şekle ne kadar uygulandığını ayarlar. Nokta biriminde.

Bakınız [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBottomBevelWidth(double value) {#setBottomBevelWidth-double-}
```
public void setBottomBevelWidth(double value)
```


Alt köşe eğiminin genişliğini, yani şekle ne kadar uygulandığını ayarlar. Nokta biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setContourColor(CellsColor value) {#setContourColor-com.aspose.cells.CellsColor-}
```
public void setContourColor(CellsColor value)
```


Bir şeklin kontur rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setContourWidth(double value) {#setContourWidth-double-}
```
public void setContourWidth(double value)
```


Şeklin kontur genişliğini, nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setExtrusionColor(CellsColor value) {#setExtrusionColor-com.aspose.cells.CellsColor-}
```
public void setExtrusionColor(CellsColor value)
```


Bir şeklin ekstrüzyon rengini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setExtrusionHeight(double value) {#setExtrusionHeight-double-}
```
public void setExtrusionHeight(double value)
```


Şekle uygulanan ekstrüzyon yüksekliğini, nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLightAngle(double value) {#setLightAngle-double-}
```
public void setLightAngle(double value)
```


Ekstrüzyon ışıklarının açısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setLighting(int value) {#setLighting-int-}
```
public void setLighting(int value)
```


Işık setinin tipini ayarlar.

Bkz [LightRigType](../../com.aspose.cells/lightrigtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLightingDirection(int value) {#setLightingDirection-int-}
```
public void setLightingDirection(int value)
```


Işık setinin sahneye göre yönlendirildiği yönü ayarlar.

Bakınız [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaterial(int value) {#setMaterial-int-}
```
public void setMaterial(int value)
```


Şeklin son görünüm ve hissini sağlamak için aydınlatma özellikleriyle birleştirilen ön ayar malzemeyi temsil eder.

Bkz [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPerspective(double value) {#setPerspective-double-}
```
public void setPerspective(double value)
```


Bir ThreeDFormat nesnesinin görüntülenebileceği açıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setPresetCameraType(int value) {#setPresetCameraType-int-}
```
public void setPresetCameraType(int value)
```


Ekstrüzyon ön ayar kamera tipini ayarlar.

Bakınız [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRotationX(double value) {#setRotationX-double-}
```
public void setRotationX(double value)
```


Ekstrüde edilmiş şeklin x ekseni etrafındaki dönüşünü derece cinsinden ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setRotationY(double value) {#setRotationY-double-}
```
public void setRotationY(double value)
```


Ekstrüde şeklin y-eksenindeki dönüşünü derece cinsinden ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setRotationZ(double value) {#setRotationZ-double-}
```
public void setRotationZ(double value)
```


Ekstrüde şeklin z-eksenindeki dönüşünü derece cinsinden ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTopBevelHeight(double value) {#setTopBevelHeight-double-}
```
public void setTopBevelHeight(double value)
```


Üst köşe eğiminin yüksekliğini, yani şekle ne kadar uygulandığını ayarlar. Nokta biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setTopBevelType(int value) {#setTopBevelType-int-}
```
public void setTopBevelType(int value)
```


Üst köşe eğiminin tipini, yani şekle ne kadar uygulandığını ayarlar. Nokta biriminde.

Bakınız [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTopBevelWidth(double value) {#setTopBevelWidth-double-}
```
public void setTopBevelWidth(double value)
```


Üst köşe eğiminin genişliğini, yani şekle ne kadar uygulandığını ayarlar. Nokta biriminde.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setZ(double value) {#setZ-double-}
```
public void setZ(double value)
```


3D şekil için yerden mesafeyi tanımlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

