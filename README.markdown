# Módulo de Autoevaluación Docente - Primaria

Este proyecto es un módulo de autoevaluación interactivo diseñado para docentes de nivel primaria que se preparan para la Promoción Horizontal 2025-2026, basado en el *Cuadernillo C2*. Es una aplicación web autónoma, creada con HTML, JavaScript y Tailwind CSS, que funciona offline y está optimizada para GitHub Pages.

## Características
- **Modos de Práctica**: 
  - Rápido (20s por pregunta, nivel R)
  - Estándar (30s por pregunta, nivel E)
  - Profesional (45s por pregunta, nivel P)
- **Interfaz Responsiva**: Compatible con dispositivos móviles y de escritorio.
- **Panel Administrativo**: Permite editar preguntas (contraseña: `Vader2025`).
- **Uso Offline**: Todo el código y las preguntas están embebidas en un solo archivo HTML.
- **Progreso y Retroalimentación**: Barra de progreso, temporizador y retroalimentación detallada por pregunta.

## Cómo Subir a GitHub Pages
1. **Crea un Repositorio en GitHub**:
   - Inicia sesión en [GitHub](https://github.com).
   - Crea un nuevo repositorio (por ejemplo, `autoevaluacion-docente`).
   - Asegúrate de que el repositorio sea público para usar GitHub Pages.

2. **Sube los Archivos**:
   - Clona el repositorio a tu máquina: `git clone <URL_DEL_REPOSITORIO>`.
   - Copia los archivos `self-assessment.html` y `README.md` al directorio del repositorio.
   - Confirma y sube los cambios:
     ```bash
     git add .
     git commit -m "Subir módulo de autoevaluación"
     git push origin main
     ```

3. **Configura GitHub Pages**:
   - Ve a la pestaña **Settings** de tu repositorio.
   - Desplázate a la sección **Pages**.
   - En **Source**, selecciona la rama `main` y la carpeta `/ (root)`.
   - Haz clic en **Save**.
   - GitHub generará una URL (por ejemplo, `https://<TU_USUARIO>.github.io/autoevaluacion-docente`).

4. **Accede al Módulo**:
   - Una vez que GitHub Pages procese los archivos (puede tomar unos minutos), visita la URL generada.
   - El módulo estará disponible para su uso en cualquier navegador.

## Cómo Usar el Módulo
1. **Inicio**:
   - Selecciona un modo de práctica: Rápido, Estándar o Profesional.
   - Cada modo presenta 10 preguntas aleatorias del nivel correspondiente (R, E o P).
2. **Responder Preguntas**:
   - Lee la pregunta y selecciona una opción dentro del tiempo límite.
   - Recibirás retroalimentación inmediata (correcto/incorrecto) con una explicación.
3. **Resultados**:
   - Al finalizar, verás tu puntaje (por ejemplo, "8 de 10").
   - Puedes reiniciar el cuestionario desde la pantalla de resultados.
4. **Panel Administrativo**:
   - Haz clic en "Acceso Administrador" e ingresa la contraseña `Vader2025`.
   - Filtra preguntas por nivel (R, E, P o todas) y edita el texto, opciones o retroalimentación directamente.

## Notas
- **Banco de Preguntas**: Actualmente, el módulo incluye 48 preguntas de nivel R. Para alcanzar las 600+ preguntas requeridas, agrega más preguntas al array `questions` en `self-assessment.html` o proporciona un JSON con las preguntas adicionales.
- **Uso Offline**: Descarga `self-assessment.html` y ábrelo en un navegador para usarlo sin conexión.
- **Compatibilidad**: Probado en Chrome, Firefox, Safari y navegadores móviles.

## Estructura de Archivos
- `self-assessment.html`: Aplicación principal con el código HTML, CSS y JavaScript.
- `README.md`: Este archivo de documentación.

## Contribuir
Si deseas agregar más preguntas o mejorar el módulo:
1. Edita el array `questions` en `self-assessment.html` con el formato `{ id, level, text, options, correct, feedback }`.
2. Crea un *pull request* con tus cambios.

## Licencia
Este proyecto es de uso libre para fines educativos. No se garantiza su uso para otros propósitos.