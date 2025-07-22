# SOCIAL OPLESK
### 
<br/>
# como instalar wsl y actualizarlo

Para **instalar y actualizar WSL (Windows Subsystem for Linux)** en tu PC con Windows 10 o Windows 11, sigue estos pasos:

**Requisitos previos**

- Debes tener Windows 10 versión 2004 o posterior (compilación 19041+) o cualquier versión de Windows 11 para usar la instalación simplificada de WSL.


### Instalación de WSL

1. **Abrir PowerShell o Símbolo del sistema en modo administrador**
Haz clic derecho sobre el acceso y selecciona "Ejecutar como administrador".
2. **Ejecutar el comando de instalación**
Para instalar WSL y la distribución por defecto (Ubuntu), usa:

```
wsl --install
```

Si deseas otra distribución, puedes ver la lista disponible con:

```
wsl --list --online
```

Y luego instalar la que prefieras, por ejemplo:

```
wsl --install -d Debian
```

Reinicia el computador cuando lo indique el instalador. Esto **habilitará todas las características necesarias, descargará el kernel y dejará WSL listo para usar.

### Actualizar WSL

- Para actualizar WSL a la última versión disponible desde la Microsoft Store o para asegurarte de tener las mejoras más recientes, ejecuta:

```
wsl --update
```

Puedes verificar la versión instalada con:

```
wsl --version
```

Esto garantiza que tienes el Subsistema de Windows para Linux más nuevo y, de ser aplicable, también se actualiza el kernel de Linux que usa WSL.


### Actualizar la distribución de Linux (opcional)

- Si también deseas actualizar la propia distribución de Linux (por ejemplo, de Ubuntu 20.04 a 22.04) dentro de WSL, sigue los comandos clásicos de actualización de cada distribución. Para Ubuntu, normalmente se usan:

```
sudo apt update && sudo apt upgrade
sudo do-release-upgrade
```

Esto actualiza los paquetes y puede cambiar la versión principal de la distribución.


### Cambiar a WSL 2 (si tienes WSL 1)

- Para verificar la versión de WSL en uso:

```
wsl -l -v
```

- Para cambiar una distribución específica a WSL 2:

```
wsl --set-version <NombreDistro> 2
```

Por ejemplo:

```
wsl --set-version Ubuntu-20.04 2
```

Eso asigna el motor WSL 2, que tiene mejor compatibilidad y rendimiento.

**Notas adicionales**

- Si usas una versión antigua de Windows o WSL, puede que necesites habilitar manualmente los componentes opcionales “VirtualMachinePlatform” y descargar e instalar el kernel de Linux por separado.
- Asegúrate de reiniciar el PC después de cualquier cambio importante de características o actualización de componentes.

Siguiendo estos pasos tendrás **WSL instalado y actualizado** a la última versión en tu sistema Windows.

<div style="text-align: center">⁂</div>
