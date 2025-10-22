##add method
## add(self, cell_name) {#System.String}
Adds a comment to the collection.
### Returns
[`Comment`](/cells/python-net/aspose.cells/comment) object index.
```python
def add(self, cell_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cell_name | System.String | Cell name. |
### Example
```python
commentIndex2 = comments.add("B2")
comment2 = comments[commentIndex2]
comment2.note = "Second note."
comment2.font.name = "Times New Roman"
```
## add(self, row, column) {#int-int}
Adds a comment to the collection.
### Returns
[`Comment`](/cells/python-net/aspose.cells/comment) object index.
```python
def add(self, row, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | int | Cell row index. |
| column | int | Cell column index. |
### Example
```python
commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"
```
### See Also
* module [`aspose.cells`](../../)
* class [`Comment`](/cells/python-net/aspose.cells/comment)
* class [`CommentCollection`](/cells/python-net/aspose.cells/commentcollection)
