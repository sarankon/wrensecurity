# Wren Security / Project Status

[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/WrenSecurity/Lobby)

### Wren : Access Management

| Project Name | Branch | Ready Build |
| ----- | ----- | ----- |
| Wren:AM | [develop](https://github.com/WrenSecurity/wrenam/tree/develop) | ??? |
| Wren:AM | [historical/master](https://github.com/WrenSecurity/wrenam/tree/historical/master) | ??? |
| Wren:AM | [master](https://github.com/WrenSecurity/wrenam/master) | ??? |
| Wren:AM | [sustaining/13](https://github.com/WrenSecurity/wrenam/tree/sustaining/13) | ??? |
| Wren:AM | [sustaining/13.5](https://github.com/WrenSecurity/wrenam/tree/sustaining/13.5) | OK |
| Wren:AM | [sustaining/14](https://github.com/WrenSecurity/wrenam/tree/sustaining/14) | ??? |

### Wren : Directory Service

| Project Name | Branch | Ready Build |
| ----- | ----- | ----- |
| Wren:DS | [legacy/master](https://github.com/WrenSecurity/wrends/tree/legacy/master) | ??? |
| Wren:DS | [master](https://github.com/WrenSecurity/wrends/tree/master) | ??? |
| Wren:DS | [sustaining/3.0](https://github.com/WrenSecurity/wrends/tree/sustaining/3.0) | ??? |

### Wren : Identity Management

| Project Name | Branch | Ready Build |
| ----- | ----- | ----- |
| Wren:IDM | [develop](https://github.com/WrenSecurity/wrenidm/tree/develop) | ??? |
| Wren:IDM | [historical/master](https://github.com/WrenSecurity/wrenidm/tree/historical/master) | ??? |
| Wren:IDM | [historical/release/4.5.0](https://github.com/WrenSecurity/wrenidm/tree/historical/release/4.5.0) | ??? |
| Wren:IDM | [historical/release/5.0.0](https://github.com/WrenSecurity/wrenidm/tree/historical/release/5.0.0) | OK |

### Wren : Identity Gateway

| Project Name | Branch | Ready Build |
| ----- | ----- | ----- |
| Wren:IG | ??? | ??? |

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

