##GridDesktop.StartFormatPainter
GridDesktop method. Notifies GridDesktop to start FormatPainter
## GridDesktop.StartFormatPainter method
Notifies GridDesktop to start FormatPainter.
```csharp
public void StartFormatPainter(bool formatOnce)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formatOnce | Boolean | if formatOnce is true,FormatPainter can use once, if formatOnce is false,FormatPainter can use multi-times,until invokes EndFormatPainter(). |
### Examples
```csharp
[C#]
gridDesktop1.StartFormatPainter(true);
[Visual Basic]
gridDesktop1.StartFormatPainter(True)
```
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
