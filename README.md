# Wren Security / Project Status

[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/WrenSecurity/Lobby)

### Wren : Access Management

| Project Name | Branch | Builds with WrenSec-Deps | Builds from JFrog |
| ----- | ----- | ----- | ----- | 
| Wren:AM | [develop](https://github.com/WrenSecurity/wrenam/tree/develop) | ??? | |
| Wren:AM | [master](https://github.com/WrenSecurity/wrenam/master) | ??? | |
| Wren:AM | [sustaining/13.x](https://github.com/WrenSecurity/wrenam/tree/sustaining/13.x) | ??? | |
| Wren:AM | [sustaining/13.5.x](https://github.com/WrenSecurity/wrenam/tree/sustaining/13.5.x) | OK | |

### Wren : Directory Service

| Project Name | Branch | Builds with WrenSec-Deps | Builds from JFrog |
| ----- | ----- | ----- | ----- | 
| Wren:DS | [feature/wrensec-builds-phase-2](https://github.com/WrenSecurity/wrends/tree/feature/wrensec-builds-phase-2) | ??? | |
| Wren:DS | [master](https://github.com/WrenSecurity/wrends/tree/master) | ??? | Testing |
| Wren:DS | [sustaining/3.x](https://github.com/WrenSecurity/wrends/tree/sustaining/3.x) | ??? | ??? |
| Wren:DS | [sustaining/3.5.x](https://github.com/WrenSecurity/wrends/tree/sustaining/3.5.x) | ??? | Testing |

### Wren : Identity Management

| Project Name | Branch | Builds with WrenSec-Deps | Builds from JFrog |
| ----- | ----- | ----- | ----- | 
| Wren:IDM | [master](https://github.com/WrenSecurity/wrenidm/tree/master) | ??? | |
| Wren:IDM | [sustaining/5.x](https://github.com/WrenSecurity/wrenidm/tree/sustaining/5.x) | OK | | 

### Wren : Identity Gateway

| Project Name | Branch | Builds with WrenSec-Deps | Builds from JFrog |
| ----- | ----- | ----- | ----- |
| Wren:IG | ??? | ??? | |

# Building Wren : Access Management

[sustaining/13.5](https://github.com/WrenSecurity/wrenam/tree/sustaining/13.5)

# Building Wren : Identity Management
### Preparing you build environment
In order to build Wren : Identity Management from source you need the following software installed:
* Ubuntu 17.04 x64
* OpenJDK 1.8 x64
* Apache Maven 3.5.0

### Building 
```
$ git clone https://github.com/WrenSecurity/wrensec-deps.git
$ cd wrensec-deps
$ ./install_openidm_5.0.0_deps.sh
$ cd ..
```

``` 
$ git clone https://github.com/WrenSecurity/wrenidm.git
$ cd wrenidm
$ git checkout historical/release/5.0.0
$ mvn package
```
After build successful you will found openidm-zip folder and openidm-5.0.0-SNAPSHOT.zip in folder

