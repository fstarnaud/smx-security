# smx-security
JAAS WindowsLoginModule OSGi Bundle for ServiceMix (Karaf)

`mvn clean install`

Copy `smx-security-1.0.jar` and `waffle.xml` files to ServiceMix `deploy` folder and launch ServiceMix. At console prompt, type:

`jaas:realm-list`

It should show:

```
Index | Realm Name | Login Module Class Name
------------------------------------------------------------------
1     | karaf      | ca.logisphere.smx.security.WindowsLoginModule
```
