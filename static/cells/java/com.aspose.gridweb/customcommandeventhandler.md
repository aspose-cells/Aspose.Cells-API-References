##CustomCommandEventHandler
Represents the interface that intend to handle Custom Command events.
**All Implemented Interfaces:**
java.io.Serializable
```
public interface CustomCommandEventHandler extends Serializable
```
Represents the interface that intend to handle Custom Command events.
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
## Methods
| Method | Description |
| --- | --- |
| [handleCellEvent(Object sender, String command)](#handleCellEvent-java.lang.Object-java.lang.String-) | handle the related Cell Event. |
### handleCellEvent(Object sender, String command) {#handleCellEvent-java.lang.Object-java.lang.String-}
```
public abstract void handleCellEvent(Object sender, String command)
```
handle the related Cell Event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | The source grid of the event. If the event if fired by a child grid's cell in hierarchical displaying mode, the sender parameter represents the child grid object. |
| command | java.lang.String | The command string user send. |
