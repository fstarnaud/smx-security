# smx-security
Waffle-based JAAS WindowsLoginModule OSGi Bundle for ServiceMix (Karaf)
Waffle is basically a wrapper for the JNA calls to SSPI. For more details see: https://github.com/Waffle/waffle

`mvn clean install`

Copy `smx-security-1.0.jar` and `waffle.xml` files to ServiceMix `deploy` folder and launch ServiceMix. At console prompt, type:

`jaas:realm-list`

It should show:

```
Index | Realm Name | Login Module Class Name
------------------------------------------------------------------
1     | karaf      | ca.logisphere.smx.security.WindowsLoginModule
```
