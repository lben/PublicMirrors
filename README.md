# PublicMirrors

Copias públicas de binarios publicados por sus proyectos originales. Los archivos se alojan como adjuntos de Releases, con enlaces al origen y checksums SHA-256.

## Graphviz 16.1.0 — EL8 / x86_64

Precompilados oficiales de Graphviz construidos para **Rocky Linux 8.9**, de la familia Enterprise Linux 8. El archivo completo contiene paquetes `16.1.0-1.el8.x86_64` y paquetes independientes de la arquitectura (`noarch`).

| Descarga | Contenido |
| --- | --- |
| [Paquetes RPM completos](https://github.com/lben/PublicMirrors/releases/download/graphviz-16.1.0-el8-x86_64/rocky_8.9_graphviz-16.1.0-rpms.tar.xz) | Archivo oficial con los RPMs, bibliotecas, plugins y paquetes opcionales. |
| [RPM único, compilado con CMake](https://github.com/lben/PublicMirrors/releases/download/graphviz-16.1.0-el8-x86_64/rocky_8.9_graphviz-16.1.0-cmake.rpm) | Empaquetado alternativo del proyecto, con sus propias dependencias. |
| [SHA256SUMS](https://github.com/lben/PublicMirrors/releases/download/graphviz-16.1.0-el8-x86_64/SHA256SUMS) | Checksums calculados después de descargar los archivos oficiales. |
| [download.sh](https://github.com/lben/PublicMirrors/releases/download/graphviz-16.1.0-el8-x86_64/download.sh) | Descarga y verifica el archivo completo desde este mirror; no instala paquetes. |

[Ver la Release del mirror](https://github.com/lben/PublicMirrors/releases/tag/graphviz-16.1.0-el8-x86_64).

### Verificación

Descarga los binarios que necesites y `SHA256SUMS` en el mismo directorio. En RHEL 8 puedes verificar los archivos descargados con:

```sh
sha256sum --check --ignore-missing SHA256SUMS
```

Se comprobaron los checksums locales y los digests internos del RPM único y de los RPMs principales (`graphviz`, `graphviz-libs`, `graphviz-nox` y `graphviz-plugins-core`). No se ha probado su ejecución en RHEL 8; la instalación depende de los repositorios y bibliotecas disponibles en el equipo de destino.

### Origen y licencias

- [Release oficial de Graphviz 16.1.0](https://gitlab.com/graphviz/graphviz/-/releases/16.1.0).
- [Archivo RPM original](https://gitlab.com/api/v4/projects/4207231/packages/generic/graphviz-releases/16.1.0/rocky_8.9_graphviz-16.1.0-rpms.tar.xz).
- [RPM CMake original](https://gitlab.com/api/v4/projects/4207231/packages/generic/graphviz-releases/16.1.0/rocky_8.9_graphviz-16.1.0-cmake.rpm).
- [Código fuente oficial de la misma versión](https://gitlab.com/api/v4/projects/4207231/packages/generic/graphviz-releases/16.1.0/graphviz-16.1.0.tar.xz).

Los binarios se redistribuyen sin modificaciones y conservan sus licencias originales. Este repositorio es un mirror independiente del proyecto Graphviz.
