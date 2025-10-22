##get_threaded_comments method
## get_threaded_comments(self, cell_name) {#System.String}
Gets the threaded comments by cell name.
### Returns
```python
def get_threaded_comments(self, cell_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cell_name | System.String | The name of the cell. |
### Example
```python
threadedComments2 = comments.get_threaded_comments("B2")
for i in range(len(threadedComments2)):
tc = threadedComments2[i]
note = tc.notes
```
## get_threaded_comments(self, row, column) {#int-int}
Gets the threaded comments by row and column index.
### Returns
```python
def get_threaded_comments(self, row, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | int | The row index. |
| column | int | The column index. |
### Example
```python
threadedComments1 = comments.get_threaded_comments(1, 1)
for i in range(len(threadedComments1)):
tc = threadedComments1[i]
note = tc.notes
```
### See Also
* module [`aspose.cells`](../../)
* class [`CommentCollection`](/cells/python-net/aspose.cells/commentcollection)
* class [`ThreadedCommentCollection`](/cells/python-net/aspose.cells/threadedcommentcollection)
