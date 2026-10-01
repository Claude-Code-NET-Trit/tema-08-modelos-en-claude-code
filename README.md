# Tema 8 · Modelos en Claude Code

Octavo tema del curso **[Claude Code .NET](https://www.trainingit.es/producto/claude-code-net/)** de TrainingIT.

En este tema aprendemos a recuperar sesiones anteriores y a controlar el consumo. `--continue` y `--resume` retoman conversaciones, y `/model` y `/effort` ajustan la capacidad del modelo y la profundidad de su razonamiento según la tarea. Con `/usage` vemos el coste y el uso por modelo en un laboratorio que planifica con Opus e implementa con Sonnet.

## Qué contiene este repositorio

| Carpeta | Descripción |
|---|---|
| `proyecto-video-8.4/` | El proyecto del curso tal como queda al terminar el vídeo 8.4 |

Úsalo para comparar con tu propio proyecto o para continuar si te has quedado atascado.

## Cómo ejecutar el proyecto

En el vídeo 8.4 la configuración privada pasa a un archivo `appsettings.Local.json` que no se sube al repositorio. Por eso, antes de arrancar la API tienes que crearlo:

1. Copia `src/MasterNet.WebApi/appsettings.Local.example.json` en la misma carpeta con el nombre `appsettings.Local.json`.
2. Sustituye su contenido por los valores que se usan en el curso:

```json
{
  "TokenKey": "c3e6e550-d9cf-4795-8b6a-c40ba0eecf24",
  "ConnectionStrings": {
    "SqlServerDatabase": "Server=localhost,1433;Initial Catalog=MasterNetDB;User ID=sa;Password=Vaxi$2025USPass;Trust Server Certificate=True;"
  }
}
```

La contraseña debe coincidir con la de `docker-compose.yml`.

## Vídeos del tema

**8.1 Resume y continue en Claude Code.** `--continue` retoma la última sesión y `--resume` permite elegir cualquiera; `/rewind` retrocede dentro de la sesión actual y `/clear` empieza de cero.

**8.2 Modelos de IA en Claude Code.** Cada modelo equilibra capacidad, velocidad y coste: Opus para analizar, Sonnet para implementar y Haiku para tareas sencillas.

**8.3 Efforts en Claude Code.** El nivel de esfuerzo fija cuánto razona el modelo; ultrathink aumenta la profundidad solo para un prompt concreto.

**8.4 Costes de Claude Code y desarrollo de proyectos.** `/usage` y las estadísticas desglosan el coste y el consumo por modelo, aplicados a una mejora real del proyecto planificada con Opus e implementada con Sonnet.

**8.5 Archivos de prompts en Claude Code.** La variable EDITOR apuntando a Neovim permite escribir prompts largos con Ctrl+G sin salir del terminal.

---

Curso **Claude Code .NET** · [TrainingIT](https://www.trainingit.es/producto/claude-code-net/)
