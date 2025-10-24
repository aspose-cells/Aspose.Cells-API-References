##CoWorkUserProvider
Represents the user provider inerface in collabration mode.only available in java version now will be available in .netython version in future.
```
public interface CoWorkUserProvider
```
Represents the user provider inerface in collabration mode.only available in java version now, will be available in .net/python version in future. Customer application can implement this interface to provide the user information.
## Methods
| Method | Description |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | Gets the unique identifier of the current user |
| [getCurrentUserName()](#getCurrentUserName--) | Gets the username of the current user |
| [getPermission()](#getPermission--) | Gets the permission level of the current user |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```
Gets the unique identifier of the current user
**Returns:**
long - Current user ID
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```
Gets the username of the current user
**Returns:**
java.lang.String - Current username
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```
Gets the permission level of the current user
**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Current user permission level
