---
title: "IconSet"
second_title: "Aspose.Cells for Java API 参考"
description: "描述 IconSet 条件格式规则。"
type: docs
url: /zh/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

描述 IconSet 条件格式规则。此条件格式规则根据单元格的值为其应用图标。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Icon Set
         IconSet iconSet = cond.getIconSet();
 
         //Set Icon Type
         iconSet.setType(IconSetType.ARROWS_3);
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | 从集合中获取[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) |
| [getCfvos()](#getCfvos--) | 获取 CFValueObjects 实例。 |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | 获取指示是否反转此图标集默认图标顺序的标志。 |
| [getShowValue()](#getShowValue--) | 获取指示是否显示此图标集所应用单元格值的标志。 |
| [getType()](#getType--) | 获取要显示的图标集类型。 |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | 指示图标集是否为自定义。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | 设置指示是否反转此图标集默认图标顺序的标志。 |
| [setShowValue(boolean value)](#setShowValue-boolean-) | 设置指示是否显示此图标集所应用单元格值的标志。 |
| [setType(int value)](#setType-int-) | 设置要显示的图标集类型。 |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


从集合中获取[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon)

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


获取 CFValueObjects 实例。

**Returns:**
[ConditionalFormattingValueCollection](../../com.aspose.cells/conditionalformattingvaluecollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getReverse() {#getReverse--}
```
public boolean getReverse()
```


获取指示是否反转此图标集默认图标顺序的标志。默认值为 false。

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


获取指示是否显示此图标集所应用单元格值的标志。默认值为 true。

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


获取要显示的图标集类型。设置该类型时将自动检查当前 Cfvos 的数量是否符合新类型。如果不符合，将清除旧的 Cfvos 并添加默认的 Cfvos。

参见[IconSetType](../../com.aspose.cells/iconsettype)。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCustom() {#isCustom--}
```
public boolean isCustom()
```


指示图标集是否为自定义。默认值为 false。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setReverse(boolean value) {#setReverse-boolean-}
```
public void setReverse(boolean value)
```


设置指示是否反转此图标集默认图标顺序的标志。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


设置指示是否显示此图标集所应用单元格值的标志。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


设置要显示的图标集类型。设置该类型时将自动检查当前 Cfvos 的数量是否符合新类型。如果不符合，将清除旧的 Cfvos 并添加默认的 Cfvos。

参见[IconSetType](../../com.aspose.cells/iconsettype)。

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

