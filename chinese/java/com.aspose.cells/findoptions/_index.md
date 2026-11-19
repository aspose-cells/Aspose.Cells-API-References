---
title: "FindOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示查找选项。"
type: docs
url: /zh/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

表示查找选项。

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | 指示搜索的字符串是否区分大小写。 |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | 获取一个值，指示是否将搜索的字符串值转换为数值数据。 |
| [getLookAtType()](#getLookAtType--) | 查看类型。 |
| [getLookInType()](#getLookInType--) | 搜索位置类型。 |
| [getRange()](#getRange--) | 获取并设置搜索范围。 |
| [getRegexKey()](#getRegexKey--) | 指示搜索的键是否为正则表达式。 |
| [getSearchBackward()](#getSearchBackward--) | 是否向后搜索单元格。 |
| [getSearchNext()](#getSearchNext--) | 搜索顺序。 |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | 指示搜索是按行还是按列进行。 |
| [getStyle()](#getStyle--) | 要搜索的格式。 |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | 指示搜索的单元格值类型是否应与搜索键相同。 |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | 指示是否已设置搜索范围。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | 指示搜索的字符串是否区分大小写。 |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | 设置一个值，以指示是否将搜索的字符串值转换为数值数据。 |
| [setLookAtType(int value)](#setLookAtType-int-) | 查看类型。 |
| [setLookInType(int value)](#setLookInType-int-) | 搜索位置类型。 |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | 设置搜索范围。 |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | 指示搜索的键是否为正则表达式。 |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | 是否向后搜索单元格。 |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | 搜索顺序。 |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | 指示搜索是按行还是按列进行。 |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | 要搜索的格式。 |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | 指示搜索的单元格值类型是否应与搜索键相同。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
```


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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


指示搜索的字符串是否区分大小写。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


获取一个值，指示是否将搜索的字符串值转换为数值数据。

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


查看类型。

参见 [LookAtType](../../com.aspose.cells/lookattype)。

**Remarks**

当 [getRegexKey()](../../com.aspose.cells/findoptions\\#getRegexKey--) 为 true 且用户已为正则表达式指定了精确规则时，出于性能考虑，应将此属性设置为 [LookAtType.ENTIRE\\_CONTENT](../../com.aspose.cells/lookattype\\#ENTIRE-CONTENT)。否则我们将重构搜索键，以确保它能够按照特定类型匹配。例如，当类型为 [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\\#CONTAINS)（此属性的默认值）时，我们会自动在搜索键的开头和结尾添加通配符。在这种情况下，正则表达式将变得更复杂，性能也会下降。

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


搜索位置类型。

参见 [LookInType](../../com.aspose.cells/lookintype)。

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


获取并设置搜索范围。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


指示搜索键是否为正则表达式。如果为 true，搜索键将被视为正则表达式并进行解析。否则，键将按照 MS Excel 的规则进行解析。

**Remarks**

即使搜索键已指定为正则表达式，它仍可能根据指定的 [getLookAtType()](../../com.aspose.cells/findoptions\\#getLookAtType--) 进行重构。例如，当类型为 [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\\#CONTAINS)（此选项的默认值）时，通配符会自动添加到搜索键的开头和结尾，以确保匹配以 “contains” 方式检查。在这种情况下，正则表达式会变得更复杂，性能也会下降。因此，出于性能考虑，如果用户已为正则表达式指定了精确规则，则无需将 [getLookAtType()](../../com.aspose.cells/findoptions\\#getLookAtType--) 用作额外约束，用户可以将其设置为 [LookAtType.ENTIRE\\_CONTENT](../../com.aspose.cells/lookattype\\#ENTIRE-CONTENT) 以获得更好的性能。

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


是否向后搜索单元格。

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


搜索顺序。True：搜索下一个。False：搜索上一个。

**Remarks**

注意：此成员现已过时。请改用 FindOptions.SearchBackward 属性。该属性将在自 2018 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


指示搜索是按行还是按列进行。

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


要搜索的格式。

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


指示搜索的单元格值类型是否应与搜索键相同。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


指示是否已设置搜索范围。

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


指示搜索的字符串是否区分大小写。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


设置一个值，以指示是否将搜索的字符串值转换为数值数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


查看类型。

参见 [LookAtType](../../com.aspose.cells/lookattype)。

**Remarks**

当 [getRegexKey()](../../com.aspose.cells/findoptions\\#getRegexKey--) 为 true 且用户已为正则表达式指定了精确规则时，出于性能考虑，应将此属性设置为 [LookAtType.ENTIRE\\_CONTENT](../../com.aspose.cells/lookattype\\#ENTIRE-CONTENT)。否则我们将重构搜索键，以确保它能够按照特定类型匹配。例如，当类型为 [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\\#CONTAINS)（此属性的默认值）时，我们会自动在搜索键的开头和结尾添加通配符。在这种情况下，正则表达式将变得更复杂，性能也会下降。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


搜索位置类型。

参见 [LookInType](../../com.aspose.cells/lookintype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


设置搜索范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 搜索范围。 |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


指示搜索键是否为正则表达式。如果为 true，搜索键将被视为正则表达式并进行解析。否则，键将按照 MS Excel 的规则进行解析。

**Remarks**

即使搜索键已指定为正则表达式，它仍可能根据指定的 [getLookAtType()](../../com.aspose.cells/findoptions\\#getLookAtType--) 进行重构。例如，当类型为 [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\\#CONTAINS)（此选项的默认值）时，通配符会自动添加到搜索键的开头和结尾，以确保匹配以 “contains” 方式检查。在这种情况下，正则表达式会变得更复杂，性能也会下降。因此，出于性能考虑，如果用户已为正则表达式指定了精确规则，则无需将 [getLookAtType()](../../com.aspose.cells/findoptions\\#getLookAtType--) 用作额外约束，用户可以将其设置为 [LookAtType.ENTIRE\\_CONTENT](../../com.aspose.cells/lookattype\\#ENTIRE-CONTENT) 以获得更好的性能。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


是否向后搜索单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


搜索顺序。True：搜索下一个。False：搜索上一个。

**Remarks**

注意：此成员现已过时。请改用 FindOptions.SearchBackward 属性。该属性将在自 2018 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


指示搜索是按行还是按列进行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


要搜索的格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


指示搜索的单元格值类型是否应与搜索键相同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

