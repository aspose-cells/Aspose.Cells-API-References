##Aspose::Cells::Cells::SetMemorySetting method
'Aspose::Cells::Cells::SetMemorySetting method. Gets or sets the memory usage option for this cells in C++.'
## Cells::SetMemorySetting method
Gets or sets the memory usage option for this cells.
```cpp
void Aspose::Cells::Cells::SetMemorySetting(MemorySetting value)
```
## Remarks
Notable limits and recommended operations for some modes: <table><tr><th>Mode </th><th>Remarks </th><th>Supported  </th></tr><tr><td>MemorySetting.MemoryPreference</td><td>Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly </td><td>v8.0.0  </td></tr><tr><td>MemorySetting.FileCache</td><td>When this mode is used for any worksheet in one workbook, Workbook.Dispose() should be called at the end of work to release all resources such as the temporary files.
Randomly accessing cells will give poor performance because data needs to be read/updated randomly and repeatedly(so the pointer in the file will be
changed accordingly and IO operations will be required repeatedly). If possible, please always access the data sequentially(row by row).
When the data of one row/cell be changed, data of other cells/rows may also be influenced(such as the data be shifted/moved to other places to allocated enough spaces for the changed data). So every change of every data requires synchronization of other existing objects(
such as Row or Cell object). So, to get better performance, please do not maintain multiple Rows/Cells at the same time. Processing them one by one will reduce the data synchronization for them so the performance can be improved a bit.  </td><td>v25.7  </td></tr></table>
## See Also
* Class [Vector](../../vector/)
* Enum [MemorySetting](../../memorysetting/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
