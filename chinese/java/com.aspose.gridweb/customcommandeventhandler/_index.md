---
title: "CustomCommandEventHandler"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于处理 Custom Command 事件的接口。"
type: docs
url: /zh/java/com.aspose.gridweb/customcommandeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```

表示用于处理 Custom Command 事件的接口。

**Example**

```
         class MyCustomCommandEventHandler implements  CustomCommandEventHandler,Serializable{
          	 public void handleCellEvent(Object sender, String command){
                         GridWebBean gridweb=(GridWebBean)sender;
          			  GridWorksheet sheet = gridweb.getActiveSheet();
         	 //Identifying a specific button by checking its command
            if (command.equals("MyButton"))
             {
                 //Accessing the cells collection of the worksheet that is currently active
                 //Putting value to "A1" cell
                  sheet.getCells().get("A1").putValue("My Custom Command Button is Clicked.");
                // System.out.println("My Custom Command Button is Clicked:"+sheet.getName()+" "+sheet.getCells().get("A1").getValue());
             }	
         }
          }
         GridWebBean gridweb=ExtPage.getInstance().getBean();
         gridweb.CustomCommand = new MyCustomCommandEventHandler();
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | 处理相关的单元格事件。 |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```


处理相关的单元格事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 发送者 | java.lang.Object | 事件的源网格。如果事件是由层次显示模式下子网格的单元格触发的，sender 参数表示子网格对象。 |
| 命令 | java.lang.String | 用户发送的命令字符串。 |

