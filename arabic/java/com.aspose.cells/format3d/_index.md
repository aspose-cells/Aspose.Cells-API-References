---
title: "Format3D"
second_title: "Aspose.Cells for Java API Reference"
description: "هذه الفئة تحدد خصائص الشكل ثلاثي الأبعاد لعنصر مخطط أو شكل."
type: docs
url: /ar/java/com.aspose.cells/format3d/
---

**Inheritance:**
java.lang.Object
```
public class Format3D
```

هذه الفئة تحدد خصائص الشكل ثلاثي الأبعاد لعنصر مخطط أو شكل.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLightingAngle()](#getLightingAngle--) | يحصل على زاوية الإضاءة. |
| [getSurfaceLightingType()](#getSurfaceLightingType--) | يحصل على نوع الإضاءة الذي سيُطبق على مشهد الشكل. |
| [getSurfaceMaterialType()](#getSurfaceMaterialType--) | يحصل على نوع المادة الذي يُدمج مع خصائص الإضاءة لإعطاء المظهر والشعور النهائي للشكل. |
| [getTopBevel()](#getTopBevel--) | يحصل على كائن [Bevel](../../com.aspose.cells/bevel) الذي يحتوي على الخصائص المرتبطة بتعريف الحافة على الوجه العلوي أو الأمامي للشكل. |
| [hasTopBevelData()](#hasTopBevelData--) | يشير إلى ما إذا كان الشكل يحتوي على بيانات الحافة العلوية. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLightingAngle(double value)](#setLightingAngle-double-) | يضبط زاوية الإضاءة. |
| [setSurfaceLightingType(int value)](#setSurfaceLightingType-int-) | يضبط نوع الإضاءة الذي سيُطبق على مشهد الشكل. |
| [setSurfaceMaterialType(int value)](#setSurfaceMaterialType-int-) | يضبط نوع المادة الذي يُدمج مع خصائص الإضاءة لإعطاء المظهر والشعور النهائي للشكل. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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
### getLightingAngle() {#getLightingAngle--}
```
public double getLightingAngle()
```


يحصل على زاوية الإضاءة. النطاق من 0 إلى 359.9 درجة.

**Returns:**
double
### getSurfaceLightingType() {#getSurfaceLightingType--}
```
public int getSurfaceLightingType()
```


يحصل على نوع الإضاءة الذي سيُطبق على مشهد الشكل. القيمة الافتراضية هي LightRigType.ThreePoint.

انظر [LightRigType](../../com.aspose.cells/lightrigtype).

**Returns:**
int
### getSurfaceMaterialType() {#getSurfaceMaterialType--}
```
public int getSurfaceMaterialType()
```


يحصل على نوع المادة الذي يُدمج مع خصائص الإضاءة لإعطاء المظهر والشعور النهائي للشكل. القيمة الافتراضية هي PresetMaterialType.WarmMatte.

انظر [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Returns:**
int
### getTopBevel() {#getTopBevel--}
```
public Bevel getTopBevel()
```


يحصل على كائن [Bevel](../../com.aspose.cells/bevel) الذي يحتوي على الخصائص المرتبطة بتعريف الحافة على الوجه العلوي أو الأمامي للشكل.

**Returns:**
[Bevel](../../com.aspose.cells/bevel)
### hasTopBevelData() {#hasTopBevelData--}
```
public boolean hasTopBevelData()
```


يشير إلى ما إذا كان الشكل يحتوي على بيانات الحافة العلوية.

**Returns:**
boolean -
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




### setLightingAngle(double value) {#setLightingAngle-double-}
```
public void setLightingAngle(double value)
```


يضبط زاوية الإضاءة. النطاق من 0 إلى 359.9 درجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setSurfaceLightingType(int value) {#setSurfaceLightingType-int-}
```
public void setSurfaceLightingType(int value)
```


يضبط نوع الإضاءة الذي سيُطبق على مشهد الشكل. القيمة الافتراضية هي LightRigType.ThreePoint.

انظر [LightRigType](../../com.aspose.cells/lightrigtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSurfaceMaterialType(int value) {#setSurfaceMaterialType-int-}
```
public void setSurfaceMaterialType(int value)
```


يضبط نوع المادة الذي يُدمج مع خصائص الإضاءة لإعطاء المظهر والشعور النهائي للشكل. القيمة الافتراضية هي PresetMaterialType.WarmMatte.

انظر [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

