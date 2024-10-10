# Ejercicio 2.
 <div style="justify">
  
 ## Crear una nueva rama llamada *ejercicio2-branch* y comprobando que se encuentra en la nueva rama.
 ```bash
 bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git checkout -b ejercicio2-branch
Cambiado a nueva rama 'ejercicio2-branch'
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git branch
  ejercicio1-branch
* ejercicio2-branch
  main
 ```

 ## Se crea un nuevo archivo ".java" con el nombre *ejercicio2.java*.

```java
     public class Ejercicio2 {
     public static void main(String[] args) {
         System.out.println("Ejercicio 1 realizado.");
     }
 }    
```
## Se realiza un commit de los cambios.
```bash
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git commit -m "Se genera el ejercicio2.java y se hace el commit"
[ejercicio2-branch 1dba583] Se genera el ejercicio2.java y se hace el commit
 2 files changed, 18 insertions(+), 1 deletion(-)
 create mode 100644 Ejercicio2.java
```
## Se vuelve a la rama "main" y se fusionan con "merge".

```bash
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git checkout main
warning: unable to rmdir 'Ejercicios-git-branch-nuevo': El directorio no está vacío
Cambiado a rama 'main'
Tu rama está actualizada con 'origin/main'.
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git merge ejercicio1-branch
Actualizando 0e2cc46..b694466
Fast-forward
 Ejercicios-git-branch-nuevo |  1 +
 README.md                   | 44 +++++++++++++++++++++++++++++++++++++++++++-
 ejercicio1.java             |  5 +++++
 3 files changed, 49 insertions(+), 1 deletion(-)
 create mode 160000 Ejercicios-git-branch-nuevo
 create mode 100644 ejercicio1.java
```

```