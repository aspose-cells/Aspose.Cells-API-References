---
title: "CellEventHandler"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于处理单元格事件的接口。"
type: docs
url: /zh/java/com.aspose.gridweb/celleventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventHandler extends Serializable
```

表示用于处理单元格事件的接口。

**Example**

```
         class SortEventHandler implements   CellEventHandler,Serializable{
 
          	public void handleCellEvent(Object sender, CellEventArgs e) {
          		//System.out.println("handleCellEvent  ....");
          		GridWebBean gridweb=(GridWebBean)sender;
            		  GridWorksheet sheet = gridweb.getWorkSheets().get(0);
            		  GridWorksheet sheet1 = gridweb.getWorkSheets().get(1);
            		if (e.getArgument().toString().equals("A1")) {
            			sheet.getCells().sort(1, 0, 20, 4, 0, true,true,false);         
            		} else if (e.getArgument().toString().equals("B1")) {                   
            			sheet.getCells().sort(1, 0, 20, 4, 1, true,true,false);         
            		} else if (e.getArgument().toString().equals("C1")) {                   
            			sheet.getCells().sort(1, 0, 20, 4, 2, true,true,false);         
            		} else if (e.getArgument().toString().equals("D1")) {                   
            			sheet.getCells().sort(1, 0, 20, 4, 3, true,true,false);         
            		} else if (e.getArgument().toString().equals("1A1")) {                  
            			sheet1.getCells().sort(0, 1, 4, 7, 0, true,true,true);          
            		} else if (e.getArgument().toString().equals("1A2")) {                  
            			sheet1.getCells().sort(0, 1, 4, 7, 1, true,true,true);          
            		} else if (e.getArgument().toString().equals("1A3")) {                  
            			sheet1.getCells().sort(0, 1, 4, 7, 2, true,true,true);          
            		} else if (e.getArgument().toString().equals("1A4")) {                  
            			sheet1.getCells().sort(0, 1, 4, 7, 3, true,true,true);          
          		}
          	}
          }                                                                                      
         GridWebBean gridweb=ExtPage.getInstance().getBean();
         gridweb.CellCommand = new SortEventHandler();
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | 处理相关的单元格事件。 |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```


处理相关的单元格事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 发送者 | java.lang.Object | 事件的源网格。如果事件是由层次显示模式下子网格的单元格触发的，sender 参数表示子网格对象。 |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | 事件参数。e.Cell 是触发事件的单元格。e.Argument 包含事件的参数。 |

