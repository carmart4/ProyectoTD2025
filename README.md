# Proyecto Tratamiento de Datos 2025
Mini proyecto sobre el análisis de tickets de supermercado.

---

## 🧭 Flujo de trabajo colaborativo con rama `prueba`

Este repositorio utiliza un flujo de trabajo basado en ramas con las siguientes reglas:

- La rama `main` contiene el código estable y funcional. Solo se actualiza después de revisiones grupales.
- La rama `prueba` es el espacio de trabajo colaborativo donde todos los integrantes del equipo desarrollan y prueban sus cambios.
- El paso de `prueba` a `main` se realiza solo tras acuerdo grupal.

## 🔁 Flujo de trabajo diario para cada colaborador

1. Cambiar a la rama de trabajo:

   ```bash
   git checkout prueba # Cambiar a la rama 'prueba'.
   git pull origin prueba # Trae las actualizaciones en la nube. 
   ```

2. Realizar cambios en el proyecto.

3. Añadir y confirmar los cambios:

   ```bash
   git add .
   git commit -m "Descripción de los cambios"
   ```

4. Asegurarse de estar sincronizado antes de subir:

   ```bash
   git pull origin prueba
   ```

5. Subir los cambios:

   ```bash
   git push origin prueba
   ```
   
## ✅ Integración a main

Cuando el equipo decide que los cambios en prueba son estables:

*Un responsable ejecuta:*
  ```bash
    git checkout main
    git pull origin main
    git merge prueba
    git push origin main
  ```
    
## 🔒 Buenas prácticas
- No hacer commits directamente en main.
- Resolver conflictos de forma colaborativa.
- Utilizar mensajes de commit claros y concisos.
- Si hay cambios grandes, se pueden crear ramas individuales basadas en prueba.
