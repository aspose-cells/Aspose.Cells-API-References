##MainWeb.SessionMode
MainWeb property. Gets or sets the session mode of the grid
## MainWeb.SessionMode property
Gets or sets the session mode of the grid.
```csharp
public SessionMode SessionMode { get; set; }
```
### Remarks
There are 4 type of session mode: 1. Session(default): Use system session to store sheet data. Generally the asp.net uses InProc session state. The grid also supports "StateServer" out process session state and SQLServer session state. 2. ViewState: Use page's viewstate to store sheet data. 3. Custom: Use LoadCustomData and SheetDataUpdated events to store/recover sheet data. 4. File: store/recover sheet data in SessionStorePath. this is the suggestion way.and can keep the file always. When using SessionMode.ViewState, the grid will store some data in the page's view state. This will decrease the server's memory usage, but the page's size will be larger and it will impact the overall performance.
### Examples
```csharp
[C#]
GridWeb1.SessionMode = SessionMode.ViewState;
[Visual Basic]
GridWeb1.SessionMode = SessionMode.ViewState
```
### See Also
* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
