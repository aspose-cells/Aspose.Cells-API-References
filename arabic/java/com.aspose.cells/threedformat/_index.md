---
title: "ThreeDFormat"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل تنسيقًا ثلاثي الأبعاد للأشكال."
type: docs
url: /ar/java/com.aspose.cells/threedformat/
---

**Inheritance:**
java.lang.Object
```
public class ThreeDFormat
```

يمثل تنسيق الشكل ثلاثي الأبعاد.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomBevelHeight()](#getBottomBevelHeight--) | يحصل على ارتفاع الحافة السفلية، أو إلى أي مدى يتم تطبيقها على الشكل. |
| [getBottomBevelType()](#getBottomBevelType--) | يحصل على نوع الحافة السفلية، أو إلى أي مدى يتم تطبيقها على الشكل. |
| [getBottomBevelWidth()](#getBottomBevelWidth--) | يحصل على عرض الحافة السفلية، أو إلى أي مدى يتم تطبيقها على الشكل. |
| [getClass()](#getClass--) |  |
| [getContourColor()](#getContourColor--) | يحصل على لون الخط الخارجي على الشكل. |
| [getContourWidth()](#getContourWidth--) | يحصل على عرض الخط الخارجي على الشكل، بوحدة النقاط. |
| [getExtrusionColor()](#getExtrusionColor--) | يحصل على لون البثق على الشكل. |
| [getExtrusionHeight()](#getExtrusionHeight--) | يحصل على ارتفاع البثق المطبق على الشكل، بوحدة النقاط. |
| [getLightAngle()](#getLightAngle--) | يحصل على زاوية أضواء البثق. |
| [getLighting()](#getLighting--) | يحصل على نوع جهاز الإضاءة. |
| [getLightingDirection()](#getLightingDirection--) | يحصل على الاتجاه الذي يتم توجيه جهاز الإضاءة منه بالنسبة للمشهد. |
| [getMaterial()](#getMaterial--) | يمثل المادة المحددة مسبقًا التي تُدمج مع خصائص الإضاءة لتوفير المظهر والشعور النهائي للشكل. |
| [getPerspective()](#getPerspective--) | يحصل على الزاوية التي يمكن عرض كائن ThreeDFormat عندها. |
| [getPresetCameraType()](#getPresetCameraType--) | يحصل على نوع كاميرا الإخراج المحددة مسبقًا. |
| [getRotationX()](#getRotationX--) | يحصل على دوران الشكل المستخرج حول المحور x بالدرجات. |
| [getRotationY()](#getRotationY--) | يحصل على دوران الشكل المستخرج حول المحور y بالدرجات. |
| [getRotationZ()](#getRotationZ--) | يحصل على دوران الشكل المستخرج حول المحور z بالدرجات. |
| [getTopBevelHeight()](#getTopBevelHeight--) | يحصل على ارتفاع الحافة العلوية، أو مدى تطبيقها داخل الشكل. |
| [getTopBevelType()](#getTopBevelType--) | يحصل على نوع الحافة العلوية، أو مدى تطبيقها داخل الشكل. |
| [getTopBevelWidth()](#getTopBevelWidth--) | يحصل على عرض الحافة العلوية، أو مدى تطبيقها داخل الشكل. |
| [getZ()](#getZ--) | يحدد المسافة من الأرض للشكل ثلاثي الأبعاد. |
| [hashCode()](#hashCode--) | يحصل على قيمة التجزئة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottomBevelHeight(double value)](#setBottomBevelHeight-double-) | يضبط ارتفاع الحافة السفلية، أو مدى تطبيقها داخل الشكل. |
| [setBottomBevelType(int value)](#setBottomBevelType-int-) | يضبط نوع الحافة السفلية، أو مدى تطبيقها داخل الشكل. |
| [setBottomBevelWidth(double value)](#setBottomBevelWidth-double-) | يضبط عرض الحافة السفلية، أو مدى تطبيقها داخل الشكل. |
| [setContourColor(CellsColor value)](#setContourColor-com.aspose.cells.CellsColor-) | يضبط لون الخط الخارجي على الشكل. |
| [setContourWidth(double value)](#setContourWidth-double-) | يضبط عرض الخط الخارجي على الشكل، بوحدة النقاط. |
| [setExtrusionColor(CellsColor value)](#setExtrusionColor-com.aspose.cells.CellsColor-) | يحصل على لون البثق على الشكل. |
| [setExtrusionHeight(double value)](#setExtrusionHeight-double-) | يضبط ارتفاع الإخراج المطبق على الشكل، بوحدة النقاط. |
| [setLightAngle(double value)](#setLightAngle-double-) | يضبط زاوية أضواء الإخراج. |
| [setLighting(int value)](#setLighting-int-) | يضبط نوع جهاز الإضاءة. |
| [setLightingDirection(int value)](#setLightingDirection-int-) | يضبط الاتجاه الذي يتم توجيه جهاز الإضاءة منه بالنسبة للمشهد. |
| [setMaterial(int value)](#setMaterial-int-) | يمثل المادة المحددة مسبقًا التي تُدمج مع خصائص الإضاءة لتوفير المظهر والشعور النهائي للشكل. |
| [setPerspective(double value)](#setPerspective-double-) | يضبط الزاوية التي يمكن عرض كائن ThreeDFormat عندها. |
| [setPresetCameraType(int value)](#setPresetCameraType-int-) | يضبط نوع كاميرا الإخراج المحددة مسبقًا. |
| [setRotationX(double value)](#setRotationX-double-) | يضبط دوران الشكل المستخرج حول المحور x بالدرجات. |
| [setRotationY(double value)](#setRotationY-double-) | يضبط دوران الشكل المستخرج حول المحور y بالدرجات. |
| [setRotationZ(double value)](#setRotationZ-double-) | يضبط دوران الشكل المستخرج حول المحور z بالدرجات. |
| [setTopBevelHeight(double value)](#setTopBevelHeight-double-) | يضبط ارتفاع الحافة العلوية، أو مدى تطبيقها داخل الشكل. |
| [setTopBevelType(int value)](#setTopBevelType-int-) | يضبط نوع الحافة العلوية، أو مدى تطبيقها داخل الشكل. |
| [setTopBevelWidth(double value)](#setTopBevelWidth-double-) | يضبط عرض الحافة العلوية، أو مدى تطبيقها داخل الشكل. |
| [setZ(double value)](#setZ-double-) | يحدد المسافة من الأرض للشكل ثلاثي الأبعاد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomBevelHeight() {#getBottomBevelHeight--}
```
public double getBottomBevelHeight()
```


يحصل على ارتفاع الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

**Returns:**
double
### getBottomBevelType() {#getBottomBevelType--}
```
public int getBottomBevelType()
```


يحصل على نوع الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

انظر [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getBottomBevelWidth() {#getBottomBevelWidth--}
```
public double getBottomBevelWidth()
```


يحصل على عرض الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

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


يحصل على لون الخط الخارجي على الشكل.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getContourWidth() {#getContourWidth--}
```
public double getContourWidth()
```


يحصل على عرض الخط الخارجي على الشكل، بوحدة النقاط.

**Returns:**
double
### getExtrusionColor() {#getExtrusionColor--}
```
public CellsColor getExtrusionColor()
```


يحصل على لون البثق على الشكل.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### getExtrusionHeight() {#getExtrusionHeight--}
```
public double getExtrusionHeight()
```


يحصل على ارتفاع البثق المطبق على الشكل، بوحدة النقاط.

**Returns:**
double
### getLightAngle() {#getLightAngle--}
```
public double getLightAngle()
```


يحصل على زاوية أضواء البثق.

**Returns:**
double
### getLighting() {#getLighting--}
```
public int getLighting()
```


يحصل على نوع جهاز الإضاءة.

انظر [LightRigType](../../com.aspose.cells/lightrigtype).

**Returns:**
int
### getLightingDirection() {#getLightingDirection--}
```
public int getLightingDirection()
```


يحصل على الاتجاه الذي يتم توجيه جهاز الإضاءة منه بالنسبة للمشهد.

انظر [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Returns:**
int
### getMaterial() {#getMaterial--}
```
public int getMaterial()
```


يمثل المادة المحددة مسبقًا التي تُدمج مع خصائص الإضاءة لتوفير المظهر والشعور النهائي للشكل.

انظر [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Returns:**
int
### getPerspective() {#getPerspective--}
```
public double getPerspective()
```


يحصل على الزاوية التي يمكن عرض كائن ThreeDFormat عندها.

**Returns:**
double
### getPresetCameraType() {#getPresetCameraType--}
```
public int getPresetCameraType()
```


يحصل على نوع كاميرا الإخراج المحددة مسبقًا.

انظر [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Returns:**
int
### getRotationX() {#getRotationX--}
```
public double getRotationX()
```


يحصل على دوران الشكل المستخرج حول المحور x بالدرجات.

**Returns:**
double
### getRotationY() {#getRotationY--}
```
public double getRotationY()
```


يحصل على دوران الشكل المستخرج حول المحور y بالدرجات.

**Returns:**
double
### getRotationZ() {#getRotationZ--}
```
public double getRotationZ()
```


يحصل على دوران الشكل المستخرج حول المحور z بالدرجات.

**Returns:**
double
### getTopBevelHeight() {#getTopBevelHeight--}
```
public double getTopBevelHeight()
```


يحصل على ارتفاع الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

**Returns:**
double
### getTopBevelType() {#getTopBevelType--}
```
public int getTopBevelType()
```


يحصل على نوع الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

انظر [BevelType](../../com.aspose.cells/beveltype).

**Returns:**
int
### getTopBevelWidth() {#getTopBevelWidth--}
```
public double getTopBevelWidth()
```


يحصل على عرض الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

**Returns:**
double
### getZ() {#getZ--}
```
public double getZ()
```


يحدد المسافة من الأرض للشكل ثلاثي الأبعاد.

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


يحصل على قيمة التجزئة.

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


يضبط ارتفاع الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setBottomBevelType(int value) {#setBottomBevelType-int-}
```
public void setBottomBevelType(int value)
```


يضبط نوع الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

انظر [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBottomBevelWidth(double value) {#setBottomBevelWidth-double-}
```
public void setBottomBevelWidth(double value)
```


يضبط عرض الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setContourColor(CellsColor value) {#setContourColor-com.aspose.cells.CellsColor-}
```
public void setContourColor(CellsColor value)
```


يضبط لون الخط الخارجي على الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setContourWidth(double value) {#setContourWidth-double-}
```
public void setContourWidth(double value)
```


يضبط عرض الخط الخارجي على الشكل، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setExtrusionColor(CellsColor value) {#setExtrusionColor-com.aspose.cells.CellsColor-}
```
public void setExtrusionColor(CellsColor value)
```


يحصل على لون البثق على الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### setExtrusionHeight(double value) {#setExtrusionHeight-double-}
```
public void setExtrusionHeight(double value)
```


يضبط ارتفاع الإخراج المطبق على الشكل، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLightAngle(double value) {#setLightAngle-double-}
```
public void setLightAngle(double value)
```


يضبط زاوية أضواء الإخراج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLighting(int value) {#setLighting-int-}
```
public void setLighting(int value)
```


يضبط نوع جهاز الإضاءة.

انظر [LightRigType](../../com.aspose.cells/lightrigtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLightingDirection(int value) {#setLightingDirection-int-}
```
public void setLightingDirection(int value)
```


يضبط الاتجاه الذي يتم توجيه جهاز الإضاءة منه بالنسبة للمشهد.

انظر [LightRigDirectionType](../../com.aspose.cells/lightrigdirectiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMaterial(int value) {#setMaterial-int-}
```
public void setMaterial(int value)
```


يمثل المادة المحددة مسبقًا التي تُدمج مع خصائص الإضاءة لتوفير المظهر والشعور النهائي للشكل.

انظر [PresetMaterialType](../../com.aspose.cells/presetmaterialtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPerspective(double value) {#setPerspective-double-}
```
public void setPerspective(double value)
```


يضبط الزاوية التي يمكن عرض كائن ThreeDFormat عندها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setPresetCameraType(int value) {#setPresetCameraType-int-}
```
public void setPresetCameraType(int value)
```


يضبط نوع كاميرا الإخراج المحددة مسبقًا.

انظر [PresetCameraType](../../com.aspose.cells/presetcameratype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRotationX(double value) {#setRotationX-double-}
```
public void setRotationX(double value)
```


يضبط دوران الشكل المستخرج حول المحور x بالدرجات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setRotationY(double value) {#setRotationY-double-}
```
public void setRotationY(double value)
```


يضبط دوران الشكل المستخرج حول المحور y بالدرجات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setRotationZ(double value) {#setRotationZ-double-}
```
public void setRotationZ(double value)
```


يضبط دوران الشكل المستخرج حول المحور z بالدرجات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTopBevelHeight(double value) {#setTopBevelHeight-double-}
```
public void setTopBevelHeight(double value)
```


يضبط ارتفاع الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTopBevelType(int value) {#setTopBevelType-int-}
```
public void setTopBevelType(int value)
```


يضبط نوع الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

انظر [BevelType](../../com.aspose.cells/beveltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTopBevelWidth(double value) {#setTopBevelWidth-double-}
```
public void setTopBevelWidth(double value)
```


يضبط عرض الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setZ(double value) {#setZ-double-}
```
public void setZ(double value)
```


يحدد المسافة من الأرض للشكل ثلاثي الأبعاد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

