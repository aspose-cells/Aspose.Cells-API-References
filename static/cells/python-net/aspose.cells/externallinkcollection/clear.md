##clear method
## clear(self) {#}
Removes all external links.
```python
def clear(self):
...
```
### Remarks
When removing external links, all formulas that reference to them will be removed too because
the references become invalid.
## clear(self, update_references_as_local) {#bool}
Removes all external links.
```python
def clear(self, update_references_as_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| update_references_as_local | bool | Whether update all references of external links in formulas to references of current workbook itself. |
### Remarks
If references are required to be updated, those references of external links in formulas
will be changed to current workbook when it is possible.
For example, one cell's original formula is "='externalsource.xlam'!customfunction()",
after removing external links, the formula will become "=customfunction()";
When the original formula is "='[externalsource.xlam]Sheet1'!$A$1",
according to whether there is one sheet with name "Sheet1" in current workbook:
if true, the formula will become "=Sheet1!$A$1";
if false, the formula will become "=#REF!$A$1".
If references are not required to be updated, all formulas with references to external links
will be removed too because those references become invalid.
### See Also
* module [`aspose.cells`](../../)
* class [`ExternalLinkCollection`](/cells/python-net/aspose.cells/externallinkcollection)
