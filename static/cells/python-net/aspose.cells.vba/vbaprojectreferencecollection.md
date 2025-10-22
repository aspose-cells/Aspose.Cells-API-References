##VbaProjectReferenceCollection class
## VbaProjectReferenceCollection class
Represents all references of VBA project.
The VbaProjectReferenceCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#aspose.cells.vba.vbaprojectreference-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#aspose.cells.vba.vbaprojectreference-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#aspose.cells.vba.vbaprojectreference) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#aspose.cells.vba.vbaprojectreference-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#aspose.cells.vba.vbaprojectreference-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`add_registered_reference(self, name, libid)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_registered_reference/#system.string-system.string) | Add a reference to an Automation type library. |
| [`add_control_refrernce(self, name, libid, twiddledlibid, extended_libid)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_control_refrernce/#system.string-system.string-system.string-system.string) | Add a reference to a twiddled type library and its extended type library. |
| [`add_project_refrernce(self, name, absolute_libid, relative_libid)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_project_refrernce/#system.string-system.string-system.string) | Adds a reference to an external VBA project. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.vba/vbaprojectreferencecollection/binary_search/#aspose.cells.vba.vbaprojectreference) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")
```
### See Also
* module [`aspose.cells.vba`](..)
