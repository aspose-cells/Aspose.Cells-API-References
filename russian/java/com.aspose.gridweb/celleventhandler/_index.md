---
title: "CellEventHandler"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс, предназначенный для обработки событий ячеек."
type: docs
url: /ru/java/com.aspose.gridweb/celleventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventHandler extends Serializable
```

Представляет интерфейс, предназначенный для обработки событий ячеек.

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
## Методы

| Метод | Описание |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | Обрабатывает связанное событие ячейки. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```


Обрабатывает связанное событие ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| отправитель | java.lang.Object | Исходная сетка события. Если событие вызвано ячейкой дочерней сетки в режиме иерархического отображения, параметр sender представляет объект дочерней сетки. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | Аргумент события. e.Cell — ячейка, вызывающая событие. e.Argument содержит аргумент события. |

