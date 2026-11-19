---
title: "CellEventHandler"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الواجهة التي تهدف إلى معالجة أحداث الخلية."
type: docs
url: /ar/java/com.aspose.gridweb/celleventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventHandler extends Serializable
```

يمثل الواجهة التي تهدف إلى معالجة أحداث الخلية.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | معالجة حدث الخلية المرتبط. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```


معالجة حدث الخلية المرتبط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المرسل | java.lang.Object | شبكة المصدر للحدث. إذا تم إطلاق الحدث من خلية شبكة فرعية في وضع العرض الهرمي، فإن معامل المرسل يمثل كائن الشبكة الفرعية. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | معامل الحدث. الـ e.Cell هو الخلية التي تُطلق الحدث. الـ e.Argument يحتوي على معامل الحدث. |

