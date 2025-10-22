##Class CustomCommandButton
Aspose.Cells.GridWeb.CustomCommandButton class. Represents a custom command button in the tab bar of the GridWeb control
## CustomCommandButton class
Represents a custom command button in the tab bar of the GridWeb control.
```csharp
public class CustomCommandButton : Control, ISerializable
```
## Constructors
| Name | Description |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | Default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | Gets or sets the click event handler at client side. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | Gets or sets the command name. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | Gets or sets the rendering type of the command. The type can be command button or context menu item. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | Indicates whether to discard user input at client browser when user click this button. Could be used as an "undo" action. |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | Gets or sets the command button's image url. If sets to null or empty string, the button will only display it's text. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | Gets or sets the alternative text of the command button. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | Gets or sets the tooltip of the command button. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | Width of the button. |
## Methods
| Name | Description |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | Internal used only. |
### Examples
```csharp
[C#]
GridWebBean GridWeb1=ExtPage.getInstance().getBean();
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```
### See Also
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)
