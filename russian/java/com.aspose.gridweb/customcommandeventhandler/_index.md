---
title: "CustomCommandEventHandler"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс, предназначенный для обработки событий пользовательских команд."
type: docs
url: /ru/java/com.aspose.gridweb/customcommandeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```

Представляет интерфейс, предназначенный для обработки событий пользовательских команд.

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
## Методы

| Метод | Описание |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | Обрабатывает связанное событие ячейки. |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```


Обрабатывает связанное событие ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| отправитель | java.lang.Object | Исходная сетка события. Если событие вызвано ячейкой дочерней сетки в режиме иерархического отображения, параметр sender представляет объект дочерней сетки. |
| команда | java.lang.String | Строка команды, отправляемая пользователем. |

