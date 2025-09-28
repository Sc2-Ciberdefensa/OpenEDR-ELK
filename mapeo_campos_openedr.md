##  Mapeo de Campos EDR                                                                 


## Eventos de Procesos
| Campo               |Descripcion                                        | Tipo de Dato |
|---------------------|---------------------------------------------------|--------------|
| rawEventld          |  Identificador del tipo de evento capturado       | int          |
| time                |  Marca temporal del evento                        | datetime     |
| tickTime            |  Tiempo relativo del evento en ticks              | time         |
| process.pid         |  PID del proceso que genero el evento             | int          |
| target.pid          |  PID del proceso objetivo                         | int          |
| file.rawPath        |  Ruta del archivo involucrado                     | str          |
| hookType            |  Tipo de hook inyectado o API hookeada            | str          |
| module.rawPath      |  Ruta del modulo DLL cargado                      | str          |
| objectType          |  Tipo de objeto afectado                          | int          |
| path                |  Ruta generica asociada al evento                 | str          |
| link                |  Enlace o path relacionado                        | str          |
| user.name           |  Usuario asociado al proceso                      | str          |
| user.sid            |  SID del usuario                                  | str          |
| user.isElevated     |  Indica si el usuario tenia privilegios elevados  | bool         |
| thread.tid          |  ID del hilo asociado                             | int          |
| errType             |  Tipo de error(Error/Warning/info)                | int          |
| errMsg              |  Mensaje de error asociado                        | str          |


 ## Eventos de Sistema
| Campo                     | Descripción                                                  | Tipo de dato |
|---------------------------|--------------------------------------------------------------|--------------|
| rawEventId                | Identificador del evento                                     | int          |
| tickTime                  | Marca de tiempo (ticks del sistema)                          | time         |
| process.pid               | ID del proceso                                               | int          |
| process.parent.pid        | ID del proceso padre                                         | int          |
| process.cmdLine           | Línea de comandos usada para ejecutar el proceso             | str          |
| process.isElevated        | Indica si el proceso se ejecuta con privilegios elevados     | bool         |
| process.elevationType     | Tipo de elevación                                            | int          |
| process.imageFile.rawPath | Ruta completa de la imagen del proceso                       | str          |
| process.userSid           | SID del usuario asociado al proceso                          | str          |
| process.exitCode          | Código de salida del proceso al finalizar                    | int          |
| time                      | Tiempo del evento (campo heredado, marcado como deprecated)  | time         |
| registry.rawPath          | Ruta completa del registro afectado                          | str          |
| registry.keyNewName       | Nuevo nombre de clave de registro                            | str          |
| registry.name             | Nombre del valor del registro                                | str          |
| registry.data             | Datos almacenados en el registro                             | str          |
| registry.rawType          | Tipo de dato del valor de registro                           | int          |
| file.rawPath              | Ruta completa del archivo                                    | str          |
| file.volume.guid          | GUID del volumen del archivo                                 | str          |
| file.volume.type          | Tipo de volumen (ej: NTFS, FAT32)                            | str          |
| file.volume.device        | Dispositivo físico asociado al volumen                       | str          |
| file.rawHash              | Hash del archivo (integridad)                                | str          |
| process.creationTime      | Tiempo de creación del proceso                               | time         |
| process.deletionTime      | Tiempo de terminación del proceso                            | time         |
| process.creatorPid        | PID del proceso creador                                      | int          |
| target.pid                | ID del proceso objetivo                                      | int          |
| accessMask                | Máscara de acceso usada en la operación                      | int          |


## Eventos de Red
| Campo               | Descripción                                                               | Tipo de dato |
| ------------------- | ------------------------------------------------------------------------- | ------------ |
| rawEventId          | Identificador del evento NetMon (CONNECT_IN, OUT, LISTEN, DNS, HTTP, FTP) | int          |
| tickTime            | Marca de tiempo (ticks del sistema)                                       | time         |
| process.pid         | ID del proceso asociado a la conexión                                     | int          |
| connection.srcIp    | Dirección IP origen                                                       | str          |
| connection.srcPort  | Puerto de origen                                                          | int          |
| connection.dstIp    | Dirección IP destino                                                      | str          |
| connection.dstPort  | Puerto de destino                                                         | int          |
| connection.protocol | Protocolo de transporte (TCP/UDP)                                         | str          |
| name                | Nombre de dominio consultado en petición DNS                              | str          |
| url                 | URL solicitada en conexión HTTP                                           | str          |
| filename            | Nombre del archivo                                                        | str          |
