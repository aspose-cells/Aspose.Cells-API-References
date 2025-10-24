##is_triple_state property
## is_triple_state property
Indicates how the specified control will display Null values.
### Remarks
| Setting | Description |
| :- | :- |
| True| The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null. |
| False| (Default) The control will cycle through states for Yes and No values. Null values display as if they were No values. |
### Definition:
```python
@property
def is_triple_state(self):
...
@is_triple_state.setter
def is_triple_state(self, value):
...
```
### See Also
* module [`aspose.cells.drawing.activexcontrols`](../../)
* class [`ToggleButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
