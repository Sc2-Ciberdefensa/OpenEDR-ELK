#MAPEO DE CAMPOS EDR 

| Nombre campo en EDR |Funcion | Tipo de Dato |
|---------------------|---------------------------------------------|--------------|
| rawEventld          |  Identificador del tipo de evento capturado | int
| time                |  marca temporal del evento                  | datetime
| tickTime            |  Tiempo relativo del evento en ticks        | time
| process.pid         |  PID del proceso que genero el evento       | int
| target.pid          |  PID del proceso objetivo                   | int
| file.rawPath        |  Ruta del archivo involucrado               | String
| hookType            |  Tipo de hook inyectado o API hookeada      | String
| module.rawPath      |  Ruta del modulo DLL cargado                | String
| objectType          |  Tipo de objeto afectado                    | int
| path                |  Ruta generica asociada al evento           | String
| link                |  Enlace o path relacionado                  | String
| user.name           |  Usuario asociado al proceso                | String
| user.sid            |  SID del usuario                            | String
| user.isElevated     |  Indica si el usuario tenia privilegios elevados  | bool
| thread.tid          |  ID del hilo asociado                       | int
| errType             |  Tipo de error(Error/Warning/info)          | int
| errMsg              |  Mensaje de error asociado                  | String
