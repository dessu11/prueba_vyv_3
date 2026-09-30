# Formulario de registro - Clase 3

## Cómo abrirlo
1. Descomprima el paquete.
2. Abra registro_v1.html con doble clic. Si se abre un editor, use Abrir con > Chrome, Edge, Firefox o Safari.
3. No requiere instalación, servidor, extensiones ni conexión.
4. Use Reiniciar prueba antes de cada caso.

## Qué contiene
- registro_v1.html: versión inicial con dos errores intencionales.
- registro_v2.html: versión que corrige ambos errores.
- LEAME_DOCENTE.md: instrucciones y resultados esperados para el docente.

La cuenta se representa mediante un registro temporal visible. Recargar o reiniciar borra los registros. No hay base de datos ni cuentas reales. No se guarda la contraseña. La regla de ocho caracteres es solo el requisito didáctico de esta actividad.

## Requisitos
- RF-01: con nombre, correo válido y contraseña válida, crear la cuenta y mostrar «Registro exitoso».
- RF-02: sin correo, no crear la cuenta y mostrar «El correo es obligatorio».
- RF-03: con contraseña menor de 8 caracteres, no crear la cuenta y mostrar «La contraseña debe tener al menos 8 caracteres».

Cada prueba parte de cero. El control de duplicados, la autenticación y otros requisitos de seguridad quedan fuera del alcance.

## Pruebas para el docente
En todos los casos use el nombre Ana.

| Caso | Correo | Contraseña | v1 | v2 |
|---|---|---|---|---|
| CP-01 | ana@example.com | Abcd1234 | Registro exitoso. Cuenta creada. Caso aprobado. | Registro exitoso. Cuenta creada. Caso aprobado. |
| CP-02 | Vacío | Abcd1234 | Registro exitoso. Cuenta creada. Caso fallido. | El correo es obligatorio. Sin cuenta. Caso aprobado. |
| CP-03 | ana@example.com | Abcd123 | Registro exitoso. Cuenta creada. Caso fallido. | La contraseña debe tener al menos 8 caracteres. Sin cuenta. Caso aprobado. |

## Uso en los 90 minutos
Mantenga la agenda de la presentación. En el bloque de ejecución (45-55 min), los estudiantes prueban realmente el HTML v1 y toman capturas en lugar de copiar resultados simulados.

1. Compartir solo registro_v1.html al comienzo.
2. Ejecutar CP-01, CP-02 y CP-03. Reiniciar antes de cada uno.
3. Capturar el formulario y el panel de resultados. Nombrar las imágenes CP-02_v1.png, etc.
4. Registrar fecha, navegador/versión, HTML local y versión v1 en el comentario de ejecución.
5. Crear BUG-01 (correo vacío) y BUG-02 (contraseña de siete caracteres), vinculados a sus casos y capturas.
6. Al llegar a verificación, compartir registro_v2.html.
7. Repetir CP-02 y CP-03 y registrar EJ-02 con nuevas capturas. Conservar EJ-01.
8. Cerrar cada defecto solo después de comprobar su corrección.
9. Repetir CP-01 como comprobación de regresión del registro válido.

CAMBIO RESPECTO AL PDF: esta v2 corrige AMBOS defectos. Por tanto, pueden cerrar BUG-01 y BUG-02 después de verificar cada uno. El PDF proponía corregir únicamente BUG-01 durante la simulación. La evidencia ahora procede del comportamiento real del HTML local, aunque el producto sigue siendo una demostración académica.

## ¿Hay que subirlo al repositorio?
No es obligatorio para abrirlo, pero es conveniente para que el equipo comparta la misma versión y conserve el código junto con las issues.

En un repositorio de práctica con permisos:
1. Abrir la pestaña Code.
2. Seleccionar Add file > Upload files.
3. Cargar solo registro_v1.html al inicio (descomprimido, no el ZIP completo).
4. Escribir un mensaje como «Agregar formulario v1 para pruebas» y confirmar los cambios.
5. Si se requiere una rama y pull request, seguir ese flujo antes de distribuir la versión.
6. Más adelante, cargar registro_v2.html y confirmar «Agregar formulario v2 con validaciones».

Mantenga esta guía docente fuera del material inicial: contiene las respuestas.
GitHub muestra el código HTML en la vista del repositorio. Para ejecutar el formulario, descargue el archivo (o Code > Download ZIP), extraiga el ZIP y abra el HTML localmente. No hace falta activar GitHub Pages.

## Evidencia
La captura debe mostrar la versión, los datos relevantes, la longitud enviada, el mensaje y si se creó una cuenta. Añada la captura al comentario de ejecución o a la issue del defecto. Una issue puede enlazar el archivo y el commit correspondiente para identificar con precisión qué se probó.

Referencia: https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
