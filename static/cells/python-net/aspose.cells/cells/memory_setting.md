##memory_setting property
## memory_setting property
Gets or sets the memory usage option for this cells.
### Remarks
Notable limits and recommended operations for some modes:
| Mode | Remarks | Supported |
| :- | :- | :- |
| Cells data will be maintained in compact format
to decrease the memory cost. On other hand, the compact data also may
cause higher time cost, especially when updating the cells data,
or accessing cells/rows randomly| v8.0.0 |
|
When this mode is used for any worksheet in one workbook, |
should be called at the end of work to release all resources such as the temporary files.
|
Randomly accessing cells will give poor performance because data needs
to be read/updated randomly and repeatedly(so the pointer in the file will be
changed accordingly and IO operations will be required repeatedly).
If possible, please always access the data sequentially(row by row).
|
When the data of one row/cell be changed, data of other cells/rows
may also be influenced(such as the data be shifted/moved to other places
to allocated enough spaces for the changed data).
So every change of every data requires synchronization of other existing objects(
such as Row or Cell object).
So, to get better performance, please do not maintain multiple Rows/Cells
at the same time. Processing them one by one will reduce the data synchronization
for them so the performance can be improved a bit.
| v25.7 |
### Definition:
```python
@property
def memory_setting(self):
...
@memory_setting.setter
def memory_setting(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
* class [`MemorySetting`](/cells/python-net/aspose.cells/memorysetting)
