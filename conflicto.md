# Evidencia de conflicto en `presentacion.md`

## Descripcion
Durante el ejercicio de Git se provoco un conflicto al modificar **la misma linea** en el archivo `presentacion.md` desde dos sitios diferentes:

- **En GitHub (web)**: añadi la linea  
  `Mi película favorita: Tomorrow Land`

- **En local (mi ordenador)**: añadí la línea  
  `Mi película favorita: Matrix`

Cuando intente subir los cambios locales con `git push`, aparecio un error de *non-fast-forward*.  
Despues, al hacer `git pull origin main`, Git detecto un **conflicto en el archivo `presentacion.md`**.

---

## Conflicto
El archivo quedo asi, mostrando las marcas de conflicto que genera Git automaticamente:

<<<<<<< HEAD
Mi pelicula favorita: Matrix
=======
Mi pelicula favorita: Tomorrow Land
>>>>>>> origin/main
