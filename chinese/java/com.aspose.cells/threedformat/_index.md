---
title: "ThreeDFormat"
second_title: "Aspose.Cells for Java API 参考"
description: "表示形状的三维格式化。"
type: docs
url: /zh/java/com.aspose.cells/threedformat/
---

**Inheritance:**
java.lang.Object
```
public class ThreeDFormat
```

表示形状的三维格式化。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomBevelHeight()](#getBottomBevelHeight--) | 获取底部斜角的高度，或其在形状中应用的深度。 |
| [getBottomBevelType()](#getBottomBevelType--) | 获取底部斜角的类型，或其在形状中应用的深度。 |
| [getBottomBevelWidth()](#getBottomBevelWidth--) | 获取底部斜角的宽度，或其在形状中应用的深度。 |
| [getClass()](#getClass--) |  |
| [getContourColor()](#getContourColor--) | 获取形状的轮廓颜色。 |
| [getContourWidth()](#getContourWidth--) | 获取形状的轮廓宽度，单位为点。 |
| [getExtrusionColor()](#getExtrusionColor--) | 获取形状的挤压颜色。 |
| [getExtrusionHeight()](#getExtrusionHeight--) | 获取应用于形状的挤压高度，单位为点。 |
| [getLightAngle()](#getLightAngle--) | 获取挤压光源的角度。 |
| [getLighting()](#getLighting--) | 获取灯光装置的类型。 |
| [getLightingDirection()](#getLightingDirection--) | 获取灯光装置相对于场景的方向。 |
| [getMaterial()](#getMaterial--) | 表示预设材质，该材质与光照属性结合，以提供形状的最终外观和感觉。 |
| [getPerspective()](#getPerspective--) | 获取 ThreeDFormat 对象的可视角度。 |
| [getPresetCameraType()](#getPresetCameraType--) | 获取挤压预设相机类型。 |
| [getRotationX()](#getRotationX--) | 获取挤压形状绕 x 轴的旋转角度（单位：度）。 |
| [getRotationY()](#getRotationY--) | 获取挤压形状绕 y 轴的旋转角度（单位：度）。 |
| [getRotationZ()](#getRotationZ--) | 获取挤压形状绕 z 轴的旋转角度（单位：度）。 |
| [getTopBevelHeight()](#getTopBevelHeight--) | 获取顶部倒角的高度，或其在形状中的应用深度。 |
| [getTopBevelType()](#getTopBevelType--) | 获取顶部倒角的类型，或其在形状中的应用深度。 |
| [getTopBevelWidth()](#getTopBevelWidth--) | 获取顶部倒角的宽度，或其在形状中的应用深度。 |
| [getZ()](#getZ--) | 定义 3D 形状距地面的距离。 |
| [hashCode()](#hashCode--) | 获取哈希码。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottomBevelHeight(double value)](#setBottomBevelHeight-double-) | 设置底部倒角的高度，或其在形状中的应用深度。 |
| [setBottomBevelType(int value)](#setBottomBevelType-int-) | 设置底部倒角的类型，或其在形状中的应用深度。 |
| [setBottomBevelWidth(double value)](#setBottomBevelWidth-double-) | 设置底部倒角的宽度，或其在形状中的应用深度。 |
| [setContourColor(CellsColor value)](#setContourColor-com.aspose.cells.CellsColor-) | 设置形状的轮廓颜色。 |
| [setContourWidth(double value)](#setContourWidth-double-) | 设置形状的轮廓宽度，单位为点。 |
| [setExtrusionColor(CellsColor value)](#setExtrusionColor-com.aspose.cells.CellsColor-) | 获取形状的挤压颜色。 |
| [setExtrusionHeight(double value)](#setExtrusionHeight-double-) | 设置应用于形状的挤压高度，单位为点。 |
| [setLightAngle(double value)](#setLightAngle-double-) | 设置挤压光源的角度。 |
| [setLighting(int value)](#setLighting-int-) | 设置灯光装置的类型。 |
| [setLightingDirection(int value)](#setLightingDirection-int-) | 设置灯光装置相对于场景的方向。 |
| [setMaterial(int value)](#setMaterial-int-) | 表示预设材质，该材质与光照属性结合，以提供形状的最终外观和感觉。 |
| [setPerspective(double value)](#setPerspective-double-) | 设置 ThreeDFormat 对象的可视角度。 |
| [setPresetCameraType(int value)](#setPresetCameraType-int-) | 设置挤压预设相机类型。 |
| [setRotationX(double value)](#setRotationX-double-) | 设置挤压形状绕 x 轴的旋转角度（单位：度）。 |
| [setRotationY(double value)](#setRotationY-double-) | 设置挤压形状绕 y 轴的旋转角度（单位：度）。 |
| [setRotationZ(double value)](#setRotationZ-double-) | 设置挤压形状绕 z 轴的旋转角度（单位：度）。 |
| [setTopBevelHeight(double value)](#setTopBevelHeight-double-) | 设置顶部斜角的高度，或其在形状中的应用深度。 |
| [setTopBevelType(int value)](#setTopBevelType-int-) | 设置顶部斜角的类型，或其在形状中的应用深度。 |
| [setTopBevelWidth(double value)](#setTopBevelWidth-double-) | 设置顶部斜角的宽度，或其在形状中的应用深度。 |
| [setZ(double value)](#setZ-double-) | 定义 3D 形状距地面的距离。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomBevelHeight() {#getBottomBevelHeight--}
```
public double getBottomBevelHeight()
```


获取底部斜角的高度，或其在形状中的应用深度。单位为点。

**Returns:**
double
### getBottomBevelType() {#getBottomBevelType--}
```
public int getBottomBevelType()
```


获取底部斜角的类型，或其在形状中的应用深度。单位为点。

参见 [BevelType](../../com.aspose.cells/beveltype)。

**Returns:**
int
### getBottomBevelWidth() {#getBottomBevelWidth--}
```
public double getBottomBevelWidth()
```


获取底部斜角的宽度，或其在形状中的应用深度。单位为点。

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


获取形状的轮廓颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getContourWidth() {#getContourWidth--}
```
public double getContourWidth()
```


获取形状的轮廓宽度，单位为点。

**Returns:**
double
### getExtrusionColor() {#getExtrusionColor--}
```
public CellsColor getExtrusionColor()
```


获取形状的挤压颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getExtrusionHeight() {#getExtrusionHeight--}
```
public double getExtrusionHeight()
```


获取应用于形状的挤压高度，单位为点。

**Returns:**
double
### getLightAngle() {#getLightAngle--}
```
public double getLightAngle()
```


获取挤压光源的角度。

**Returns:**
double
### getLighting() {#getLighting--}
```
public int getLighting()
```


获取灯光装置的类型。

参见 [LightRigType](../../com.aspose.cells/lightrigtype)。

**Returns:**
int
### getLightingDirection() {#getLightingDirection--}
```
public int getLightingDirection()
```


获取灯光装置相对于场景的方向。

参见 [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype)。

**Returns:**
int
### getMaterial() {#getMaterial--}
```
public int getMaterial()
```


表示预设材质，该材质与光照属性结合，以提供形状的最终外观和感觉。

参见 [PresetMaterialType](../../com.aspose.cells/presetmaterialtype)。

**Returns:**
int
### getPerspective() {#getPerspective--}
```
public double getPerspective()
```


获取 ThreeDFormat 对象的可视角度。

**Returns:**
double
### getPresetCameraType() {#getPresetCameraType--}
```
public int getPresetCameraType()
```


获取挤压预设相机类型。

参见 [PresetCameraType](../../com.aspose.cells/presetcameratype)。

**Returns:**
int
### getRotationX() {#getRotationX--}
```
public double getRotationX()
```


获取挤压形状绕 x 轴的旋转角度（单位：度）。

**Returns:**
double
### getRotationY() {#getRotationY--}
```
public double getRotationY()
```


获取挤压形状绕 y 轴的旋转角度（单位：度）。

**Returns:**
double
### getRotationZ() {#getRotationZ--}
```
public double getRotationZ()
```


获取挤压形状绕 z 轴的旋转角度（单位：度）。

**Returns:**
double
### getTopBevelHeight() {#getTopBevelHeight--}
```
public double getTopBevelHeight()
```


获取顶部斜角的高度，或其在形状中的应用深度。单位为点。

**Returns:**
double
### getTopBevelType() {#getTopBevelType--}
```
public int getTopBevelType()
```


获取顶部斜角的类型，或其在形状中的应用深度。单位为点。

参见 [BevelType](../../com.aspose.cells/beveltype)。

**Returns:**
int
### getTopBevelWidth() {#getTopBevelWidth--}
```
public double getTopBevelWidth()
```


获取顶部斜角的宽度，或其在形状中的应用深度。单位为点。

**Returns:**
double
### getZ() {#getZ--}
```
public double getZ()
```


定义 3D 形状距地面的距离。

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


获取哈希码。

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


设置底部斜角的高度，或其在形状中的应用深度。单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setBottomBevelType(int value) {#setBottomBevelType-int-}
```
public void setBottomBevelType(int value)
```


设置底部斜角的类型，或其在形状中的应用深度。单位为点。

参见 [BevelType](../../com.aspose.cells/beveltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBottomBevelWidth(double value) {#setBottomBevelWidth-double-}
```
public void setBottomBevelWidth(double value)
```


设置底部斜角的宽度，或其在形状中的应用深度。单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setContourColor(CellsColor value) {#setContourColor-com.aspose.cells.CellsColor-}
```
public void setContourColor(CellsColor value)
```


设置形状的轮廓颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setContourWidth(double value) {#setContourWidth-double-}
```
public void setContourWidth(double value)
```


设置形状的轮廓宽度，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setExtrusionColor(CellsColor value) {#setExtrusionColor-com.aspose.cells.CellsColor-}
```
public void setExtrusionColor(CellsColor value)
```


获取形状的挤压颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setExtrusionHeight(double value) {#setExtrusionHeight-double-}
```
public void setExtrusionHeight(double value)
```


设置应用于形状的挤压高度，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLightAngle(double value) {#setLightAngle-double-}
```
public void setLightAngle(double value)
```


设置挤压光源的角度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLighting(int value) {#setLighting-int-}
```
public void setLighting(int value)
```


设置灯光装置的类型。

参见 [LightRigType](../../com.aspose.cells/lightrigtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLightingDirection(int value) {#setLightingDirection-int-}
```
public void setLightingDirection(int value)
```


设置灯光装置相对于场景的方向。

参见 [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaterial(int value) {#setMaterial-int-}
```
public void setMaterial(int value)
```


表示预设材质，该材质与光照属性结合，以提供形状的最终外观和感觉。

参见 [PresetMaterialType](../../com.aspose.cells/presetmaterialtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPerspective(double value) {#setPerspective-double-}
```
public void setPerspective(double value)
```


设置 ThreeDFormat 对象的可视角度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setPresetCameraType(int value) {#setPresetCameraType-int-}
```
public void setPresetCameraType(int value)
```


设置挤压预设相机类型。

参见 [PresetCameraType](../../com.aspose.cells/presetcameratype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRotationX(double value) {#setRotationX-double-}
```
public void setRotationX(double value)
```


设置挤压形状绕 x 轴的旋转角度（单位：度）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setRotationY(double value) {#setRotationY-double-}
```
public void setRotationY(double value)
```


设置挤压形状绕 y 轴的旋转角度（单位：度）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setRotationZ(double value) {#setRotationZ-double-}
```
public void setRotationZ(double value)
```


设置挤压形状绕 z 轴的旋转角度（单位：度）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTopBevelHeight(double value) {#setTopBevelHeight-double-}
```
public void setTopBevelHeight(double value)
```


设置顶部斜角的高度，或其在形状中的应用深度。单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTopBevelType(int value) {#setTopBevelType-int-}
```
public void setTopBevelType(int value)
```


设置顶部斜角的类型，或其在形状中的应用深度。单位为点。

参见 [BevelType](../../com.aspose.cells/beveltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTopBevelWidth(double value) {#setTopBevelWidth-double-}
```
public void setTopBevelWidth(double value)
```


设置顶部斜角的宽度，或其在形状中的应用深度。单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setZ(double value) {#setZ-double-}
```
public void setZ(double value)
```


定义 3D 形状距地面的距离。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

