##remove_at method
## remove_at(self, cell_name) {#System.String}
Removes the comment of the specific cell.
```python
def remove_at(self, cell_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cell_name | System.String | The name of cell which contains a comment. |
### Example
```python
comments.remove_at("B2")
```
## remove_at(self, row, column) {#int-int}
Removes the comment of the specific cell.
```python
def remove_at(self, row, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | int | The row index. |
| column | int | the column index. |
### Example
```python
comments.remove_at(1, 1)
```
### See Also
* module [`aspose.cells`](../../)
* class [`CommentCollection`](/cells/python-net/aspose.cells/commentcollection)
