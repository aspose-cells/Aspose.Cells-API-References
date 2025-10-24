##user_password property
## user_password property
Gets or sets the user password required for opening the encrypted PDF document.
### Remarks
The owner password or user password will be required to open an encrypted PDF document for viewing.
The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.
Opening the document with the correct owner password allows full access to the document.
Opening the document with the correct user password (or opening a document that does not have a user password)
allows limited access as the permissions specified.
### Definition:
```python
@property
def user_password(self):
...
@user_password.setter
def user_password(self, value):
...
```
### See Also
* module [`aspose.cells.rendering.pdfsecurity`](../../)
* class [`PdfSecurityOptions`](/cells/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
