---
title: "CustomCommandEventHandler"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الواجهة التي تهدف إلى معالجة أحداث Custom Command."
type: docs
url: /ar/java/com.aspose.gridweb/customcommandeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```

يمثل الواجهة التي تهدف إلى معالجة أحداث Custom Command.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | معالجة حدث الخلية المرتبط. |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```


معالجة حدث الخلية المرتبط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المرسل | java.lang.Object | شبكة المصدر للحدث. إذا تم إطلاق الحدث من خلية شبكة فرعية في وضع العرض الهرمي، فإن معامل المرسل يمثل كائن الشبكة الفرعية. |
| الأمر | java.lang.String | سلسلة الأمر التي يرسلها المستخدم. |

