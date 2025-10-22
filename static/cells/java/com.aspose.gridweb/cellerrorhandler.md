##CellErrorHandler
Represents the interface that intend to handle cell error events.
**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```
Represents the interface that intend to handle cell error events.
## Methods
| Method | Description |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | handle the related Cell Event. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```
handle the related Cell Event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | The source of the event. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | The cell operation error. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | can get onerror action type information. |
