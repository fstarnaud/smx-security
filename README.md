# smx-security
Waffle-based JAAS WindowsLoginModule OSGi Bundle for ServiceMix (Karaf). Waffle is basically a wrapper for  JNA calls to SSPI, see: https://github.com/Waffle/waffle

To build POM file, use Maven:

`mvn clean install`

Copy resulting `smx-security-1.0.jar` and `waffle.xml` files to ServiceMix `deploy` folder and launch ServiceMix. At console prompt, type:

`jaas:realm-list`

It should show:

```
Index | Realm Name | Login Module Class Name
------------------------------------------------------------------
1     | karaf      | ca.logisphere.smx.security.WindowsLoginModule
```
