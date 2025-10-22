##CellEventStringHandler
Represents the interface that intend to handle cell events.
**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```
Represents the interface that intend to handle cell events.
## Methods
| Method | Description |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | handle the related Cell Event. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```
handle the related Cell Event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | The source grid of the event. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | The event argument. The e.Cell is the cell who fires the event. The e.Argument contains the argument of the event. |
**Returns:**
java.lang.String - string value
