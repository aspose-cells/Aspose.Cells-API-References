---
title: "Format3D"
second_title: "Aspose.Cells for Java API 参考"
description: "此类指定图表元素或形状的 3D 形状属性。"
type: docs
url: /zh/java/com.aspose.cells/format3d/
---

**Inheritance:**
java.lang.Object
```
public class Format3D
```

此类指定图表元素或形状的 3D 形状属性。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLightingAngle()](#getLightingAngle--) | 获取照明角度。 |
| [getSurfaceLightingType()](#getSurfaceLightingType--) | 获取将应用于形状场景的照明类型。 |
| [getSurfaceMaterialType()](#getSurfaceMaterialType--) | 获取与照明属性结合以呈现形状最终外观和感觉的材料类型。 |
| [getTopBevel()](#getTopBevel--) | 获取 [Bevel](../../com.aspose.cells/bevel) 对象，该对象保存与在形状的顶部或前面定义斜角相关的属性。 |
| [hasTopBevelData()](#hasTopBevelData--) | 指示形状是否具有顶部斜角数据。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLightingAngle(double value)](#setLightingAngle-double-) | 设置照明角度。 |
| [setSurfaceLightingType(int value)](#setSurfaceLightingType-int-) | 设置将应用于形状场景的照明类型。 |
| [setSurfaceMaterialType(int value)](#setSurfaceMaterialType-int-) | 设置与照明属性结合以呈现形状最终外观和感觉的材料类型。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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


获取照明角度。范围为 0 到 359.9 度。

**Returns:**
double
### getSurfaceLightingType() {#getSurfaceLightingType--}
```
public int getSurfaceLightingType()
```


获取将应用于形状场景的照明类型。默认值为 LightRigType.ThreePoint。

参见 [LightRigType](../../com.aspose.cells/lightrigtype)。

**Returns:**
int
### getSurfaceMaterialType() {#getSurfaceMaterialType--}
```
public int getSurfaceMaterialType()
```


获取与照明属性结合以呈现形状最终外观和感觉的材料类型。默认值为 PresetMaterialType.WarmMatte。

参见 [PresetMaterialType](../../com.aspose.cells/presetmaterialtype)。

**Returns:**
int
### getTopBevel() {#getTopBevel--}
```
public Bevel getTopBevel()
```


获取 [Bevel](../../com.aspose.cells/bevel) 对象，该对象保存与在形状的顶部或前面定义斜角相关的属性。

**Returns:**
[Bevel](../../com.aspose.cells/bevel)
### hasTopBevelData() {#hasTopBevelData--}
```
public boolean hasTopBevelData()
```


指示形状是否具有顶部斜角数据。

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


设置照明角度。范围为 0 到 359.9 度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setSurfaceLightingType(int value) {#setSurfaceLightingType-int-}
```
public void setSurfaceLightingType(int value)
```


设置将应用于形状场景的照明类型。默认值为 LightRigType.ThreePoint。

参见 [LightRigType](../../com.aspose.cells/lightrigtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSurfaceMaterialType(int value) {#setSurfaceMaterialType-int-}
```
public void setSurfaceMaterialType(int value)
```


设置与照明属性结合以呈现形状最终外观和感觉的材料类型。默认值为 PresetMaterialType.WarmMatte。

参见 [PresetMaterialType](../../com.aspose.cells/presetmaterialtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

