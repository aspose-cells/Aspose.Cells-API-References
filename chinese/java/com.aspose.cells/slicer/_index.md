---
title: "切片器"
second_title: "Aspose.Cells for Java API 参考"
description: "切片器视图的摘要描述"
type: docs
url: /zh/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

切片器视图的摘要描述

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | 添加数据透视表连接。 |
| [clearFilter()](#clearFilter--) | 移除筛选器 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | 获取或设置切片器对象的描述性（替代）文本字符串。 |
| [getCaption()](#getCaption--) | 获取或设置指定切片器的标题。 |
| [getCaptionVisible()](#getCaptionVisible--) | 获取或设置显示切片器标题的页眉是否可见。 |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | 获取或设置切片器中每列的宽度，单位为点。 |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | 获取\u807d每列的宽度\u807d切片器中，单位为\u807dpixels。\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | 指定第一个切片器项的零基索引。 |
| [getHeight()](#getHeight--) | 获取或设置指定切片器的高度，单位为点。 |
| [getHeightPixel()](#getHeightPixel--) | 返回或设置指定切片器的高度，单位为像素。 |
| [getLeftPixel()](#getLeftPixel--) | 返回或设置切片器形状相对于其左列的水平偏移量，单位为像素。 |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | 指示是否锁定纵横比。 |
| [getLockedPosition()](#getLockedPosition--) | 指示指定的切片器是否可以通过用户界面移动或调整大小。 |
| [getName()](#getName--) | 返回或设置指定切片器的名称 |
| [getNumberOfColumns()](#getNumberOfColumns--) | 返回或设置切片器中的列数。 |
| [getParent()](#getParent--) | 返回包含此切片器的 [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) 对象。 |
| [getPlacement()](#getPlacement--) | 表示绘图对象附着在其下方单元格的方式。 |
| [getRowHeight()](#getRowHeight--) | 返回或设置指定切片器中每行的高度，单位为磅。 |
| [getRowHeightPixel()](#getRowHeightPixel--) | 返回或设置指定切片器中每行的高度，单位为像素。 |
| [getShape()](#getShape--) | 返回与指定切片器关联的 Shape 对象。 |
| [getShowAllItems()](#getShowAllItems--) | 指示是否显示所有项目，即使没有数据或已被删除。 |
| [getShowCaption()](#getShowCaption--) | 指示切片器的标题是否可见。 |
| [getShowMissing()](#getShowMissing--) | 指示是否显示已从数据源删除的项目。 |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | 指示是否显示已从数据源删除的项目。 |
| [getSlicerCache()](#getSlicerCache--) | 返回与切片器关联的 SlicerCache 对象。 |
| [getSortOrderType()](#getSortOrderType--) | 指示项目的排序类型。 |
| [getStyleType()](#getStyleType--) | 指定内置切片器样式的类型。 |
| [getTitle()](#getTitle--) | 指定当前 Slicer 对象的标题。 |
| [getTopPixel()](#getTopPixel--) | 返回或设置切片器形状相对于其顶部行的垂直偏移量，单位为像素。 |
| [getWidth()](#getWidth--) | 返回或设置指定切片器的宽度，单位为磅。 |
| [getWidthPixel()](#getWidthPixel--) | 返回或设置指定切片器的宽度，单位为像素。 |
| [getWorksheet()](#getWorksheet--) | 返回包含此切片器的 [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) 对象。 |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | 指示切片器形状是否被锁定。 |
| [isPrintable()](#isPrintable--) | 指示切片器对象是否可打印。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | 从关联的透视表刷新切片器的项目。 |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | 移除透视表连接。 |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **备注** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | 获取或设置切片器对象的描述性（替代）文本字符串。 |
| [setCaption(String value)](#setCaption-java.lang.String-) | 获取或设置指定切片器的标题。 |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | 获取或设置显示切片器标题的页眉是否可见。 |
| [setColumnWidth(double value)](#setColumnWidth-double-) | 获取或设置切片器中每列的宽度，单位为点。 |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | 设置宽度为\u807d每列在\u807d切片器，单位为\u807d像素。\u807d |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | 指定第一个切片器项的零基索引。 |
| [setHeight(double value)](#setHeight-double-) | 获取或设置指定切片器的高度，单位为点。 |
| [setHeightPixel(int value)](#setHeightPixel-int-) | 返回或设置指定切片器的高度，单位为像素。 |
| [setLeftPixel(int value)](#setLeftPixel-int-) | 返回或设置切片器形状相对于其左列的水平偏移量，单位为像素。 |
| [setLocked(boolean value)](#setLocked-boolean-) | 指示切片器形状是否被锁定。 |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | 指示是否锁定纵横比。 |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | 指示指定的切片器是否可以通过用户界面移动或调整大小。 |
| [setName(String value)](#setName-java.lang.String-) | 返回或设置指定切片器的名称 |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | 返回或设置切片器中的列数。 |
| [setPlacement(int value)](#setPlacement-int-) | 表示绘图对象附着在其下方单元格的方式。 |
| [setPrintable(boolean value)](#setPrintable-boolean-) | 指示切片器对象是否可打印。 |
| [setRowHeight(double value)](#setRowHeight-double-) | 返回或设置指定切片器中每行的高度，单位为磅。 |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | 返回或设置指定切片器中每行的高度，单位为像素。 |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | 指示是否显示所有项目，即使没有数据或已被删除。 |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | 指示切片器的标题是否可见。 |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | 指示是否显示已从数据源删除的项目。 |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | 指示是否显示已从数据源删除的项目。 |
| [setSortOrderType(int value)](#setSortOrderType-int-) | 指示项目的排序类型。 |
| [setStyleType(int value)](#setStyleType-int-) | 指定内置切片器样式的类型。 |
| [setTitle(String value)](#setTitle-java.lang.String-) | 指定当前 Slicer 对象的标题。 |
| [setTopPixel(int value)](#setTopPixel-int-) | 返回或设置切片器形状相对于其顶部行的垂直偏移量，单位为像素。 |
| [setWidth(double value)](#setWidth-double-) | 返回或设置指定切片器的宽度，单位为磅。 |
| [setWidthPixel(int value)](#setWidthPixel-int-) | 返回或设置指定切片器的宽度，单位为像素。 |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | 删除所选过滤器标签。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


添加数据透视表连接。

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


移除筛选器

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


获取或设置切片器对象的描述性（替代）文本字符串。

**Remarks**

注意：此成员现已过时。请改用 [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


获取或设置指定切片器的标题。

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


返回或设置显示切片器 Caption 的页眉是否可见。默认值为 true。

**Remarks**

注意：此成员现已过时。请改用 [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


获取或设置切片器中每列的宽度，单位为点。

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


获取\u807d每列的宽度\u807d切片器中，单位为\u807dpixels。\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


指定第一个切片器项的零基索引。

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


获取或设置指定切片器的高度，单位为点。

**Remarks**

注意：此成员现已过时。请改用 Shape.HeightPt 属性。此属性将在 2025 年 5 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


返回或设置指定切片器的高度，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Height 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


返回或设置切片器形状相对于其左列的水平偏移量，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Left 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


指示是否锁定纵横比。

**Remarks**

注意：此成员现已过时。请改用 [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) 方法。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


指示指定的切片器是否可以通过用户界面移动或调整大小。

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


返回或设置指定切片器的名称

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


返回或设置切片器中的列数。默认值为 1。

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


返回包含此切片器的 [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) 对象。只读。

**Remarks**

注意：此成员现已过时。请改用 [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


表示绘图对象附着在其下方单元格的方式。该属性控制对象在工作表上的放置位置。

参见 [PlacementType](../../com.aspose.cells/placementtype)。

**Remarks**

注意：此成员现已过时。请改用 [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


返回或设置指定切片器中每行的高度，单位为磅。

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


返回或设置指定切片器中每行的高度，单位为像素。

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


返回与指定切片器关联的 Shape 对象。只读。

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


指示即使没有数据或已删除，也显示所有项目。默认值为 true；

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


指示切片器的页眉是否可见。默认值为 true。

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


指示是否显示已从数据源删除的项目。

**Remarks**

仅在 [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) 为 true 时有效。

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


指示是否显示已从数据源删除的项目。

参见 [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode)。

**Remarks**

仅在 [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) 为 true 时有效。

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


返回与切片器关联的 SlicerCache 对象。只读。

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


指示项目的排序类型。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


指定内置切片器样式的类型。默认类型为 SlicerStyleLight1。

参见 [SlicerStyleType](../../com.aspose.cells/slicerstyletype)。

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


指定当前 Slicer 对象的标题。

**Remarks**

注意：此成员现已过时。请改用 [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


返回或设置切片器形状相对于其顶部行的垂直偏移量，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Top 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


返回或设置指定切片器的宽度，单位为磅。

**Remarks**

注意：此成员现已过时。请改用 Shape.WidthPt 属性。此属性将在 2025 年 5 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


返回或设置指定切片器的宽度，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Width 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


返回包含此切片器的 [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) 对象。只读。

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


指示切片器形状是否被锁定。

**Remarks**

注意：此成员现已过时。请改用 [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


指示切片器对象是否可打印。

**Remarks**

注意：此成员现已过时。请改用 [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
         slicer.removePivotConnection(pivot);
```

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




### refresh() {#refresh--}
```
public void refresh()
```


从关联的透视表刷新切片器的项目。

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


移除透视表连接。

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable 对象 |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

如果您想选择所有项目，请使用 [clearFilter()](../../com.aspose.cells/slicer\#clearFilter--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String[] | 已选择的标签。 |
| 追加 | boolean | False 表示仅选择这些标签并取消选择其他标签。True 表示保留之前已选择的项目并选择这些标签。 |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


获取或设置切片器对象的描述性（替代）文本字符串。

**Remarks**

注意：此成员现已过时。请改用 [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


获取或设置指定切片器的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


返回或设置显示切片器 Caption 的页眉是否可见。默认值为 true。

**Remarks**

注意：此成员现已过时。请改用 [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


获取或设置切片器中每列的宽度，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


设置宽度为\u807d每列在\u807d切片器，单位为\u807d像素。\u807d

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


指定第一个切片器项的零基索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


获取或设置指定切片器的高度，单位为点。

**Remarks**

注意：此成员现已过时。请改用 Shape.HeightPt 属性。此属性将在 2025 年 5 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


返回或设置指定切片器的高度，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Height 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


返回或设置切片器形状相对于其左列的水平偏移量，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Left 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


指示切片器形状是否被锁定。

**Remarks**

注意：此成员现已过时。请改用 [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


指示是否锁定纵横比。

**Remarks**

注意：此成员现已过时。请改用 [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) 方法。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


指示指定的切片器是否可以通过用户界面移动或调整大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


返回或设置指定切片器的名称

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


返回或设置切片器中的列数。默认值为 1。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


表示绘图对象附着在其下方单元格的方式。该属性控制对象在工作表上的放置位置。

参见 [PlacementType](../../com.aspose.cells/placementtype)。

**Remarks**

注意：此成员现已过时。请改用 [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


指示切片器对象是否可打印。

**Remarks**

注意：此成员现已过时。请改用 [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


返回或设置指定切片器中每行的高度，单位为磅。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


返回或设置指定切片器中每行的高度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


指示即使没有数据或已删除，也显示所有项目。默认值为 true；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


指示切片器的页眉是否可见。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


指示是否显示已从数据源删除的项目。

**Remarks**

仅在 [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) 为 true 时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


指示是否显示已从数据源删除的项目。

参见 [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode)。

**Remarks**

仅在 [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) 为 true 时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


指示项目的排序类型。

参见 [SortOrder](../../com.aspose.cells/sortorder)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


指定内置切片器样式的类型。默认类型为 SlicerStyleLight1。

参见 [SlicerStyleType](../../com.aspose.cells/slicerstyletype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


指定当前 Slicer 对象的标题。

**Remarks**

注意：此成员现已过时。请改用 [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) 属性。此属性将在 2026 年 1 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


返回或设置切片器形状相对于其顶部行的垂直偏移量，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Top 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


返回或设置指定切片器的宽度，单位为磅。

**Remarks**

注意：此成员现已过时。请改用 Shape.WidthPt 属性。此属性将在 2025 年 5 月起 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


返回或设置指定切片器的宽度，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Width 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

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
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


删除所选过滤器标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 标签 | java.lang.String[] | 这些标签。 |

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

