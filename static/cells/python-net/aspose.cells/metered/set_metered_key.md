##set_metered_key method
## set_metered_key(self, public_key, private_key) {#System.String-System.String}
Sets metered public and private key.
If you purchase metered license, when start application, this API should be called, normally, this is enough.
However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status,
to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.
```python
def set_metered_key(self, public_key, private_key):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| public_key | System.String | public key |
| private_key | System.String | private key |
### See Also
* module [`aspose.cells`](../../)
* class [`Metered`](/cells/python-net/aspose.cells/metered)
