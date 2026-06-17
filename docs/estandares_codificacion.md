# Estándares de Nomenclatura y Documentación – SIGA

## Convenciones de nomenclatura
- Variables y funciones: camelCase (ej. obtenerUsuario, totalRegistros).
- Clases y componentes de React: PascalCase (ej. UsuarioCard, ReporteTabla).
- Constantes globales: UPPER_SNAKE_CASE (ej. MAX_INTENTOS_LOGIN).
- Todos los nombres deben escribirse en inglés y ser descriptivos.
- Prohibido el uso de nombres genéricos como "dato1", "variable", "temp" o similares.

## Organización de archivos
- Cada archivo debe contener únicamente la lógica de su propio módulo.
- No mezclar responsabilidades de frontend y backend en un mismo archivo.

## Documentación con JSDoc
Todas las funciones públicas deben documentarse con JSDoc. Ejemplo:

/**
 * Calcula el total de registros administrativos activos.
 * @param {Array<Object>} registros - Lista de registros del sistema.
 * @returns {number} Total de registros con estado "activo".
 */
function contarRegistrosActivos(registros) {
  return registros.filter(r => r.estado === "activo").length;
}

## Revisión
El incumplimiento de estos estándares se detectará en las revisiones cruzadas y deberá corregirse antes de integrar el cambio a la rama principal.