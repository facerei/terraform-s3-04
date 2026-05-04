# REBASE.md
 
## Que es git rebase -i
 
git rebase -i permite reescribir el historial de commits de forma interactiva.
Es útil para limpiar mensajes vagos o fusionar commits pequeños antes de
compartir el trabajo con el equipo.
 
## Proceso seguido
 
### Fase 1: commits con mensajes malos
Se crearon tres commits con mensajes poco descriptivos (Arreglos, Cambios, Cosas)
para simular el trabajo rápido del día a día sin cuidar los mensajes.
 
### Fase 2: rebase interactivo
Se ejecuto git rebase -i HEAD~3. En el editor se usó:
- reword en el primer commit para cambiar su mensaje.
- squash en los otros dos para fusionarlos con el primero.
El resultado es un unico commit con el mensaje:
actualiza README.md con notas del proyecto
 
### Fase 3: push --force
Al haber reescrito el historial local fue necesario git push --force
para actualizar el remoto. Este comando sobreescribe el historial de
GitHub con el local. Se usa con cuidado en ramas compartidas.
 
## Por que es importante
 
Un historial limpio facilita las revisiones de código, la búsqueda de
errores y la colaboración. Mensajes como Arreglos no aportan contexto.
