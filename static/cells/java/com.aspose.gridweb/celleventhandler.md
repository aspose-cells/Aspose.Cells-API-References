##CellEventHandler
Represents the interface that intend to handle cell events.
**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventHandler extends Serializable
```
Represents the interface that intend to handle cell events.
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
## Methods
| Method | Description |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | handle the related Cell Event. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```
handle the related Cell Event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | The source grid of the event. If the event if fired by a child grid's cell in hierarchical displaying mode, the sender parameter represents the child grid object. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | The event argument. The e.Cell is the cell who fires the event. The e.Argument contains the argument of the event. |
