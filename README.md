# Entornos de Desarrollo: Comenzando con Git "Trabajando con Branchs"
 <div style="justify">
  
 ## Clonación de repositorio.
```bash
git clobae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git clone https://github.com/Cdiagal/Ejercicios-git-branch-nuevo
Clonando en 'Ejercicios-git-branch-nuevo'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Recibiendo objetos: 100% (3/3), listo.
```
## Crear una nueva rama llamada *ejercicio1-branch* y comprobando que se encuentra en la nueva rama.

```bash
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git checkout -b ejercicio1-branch
Cambiado a nueva rama 'ejercicio1-branch'
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git branch
* ejercicio1-branch
  main
```

## Se crea un nuevo archivo ".java" con el nombre *Ejercicio1.java*.

```java
     public class Ejercicio1 {
     public static void main(String[] args) {
         System.out.println("Ejercicio 1 realizado.");
     }
 }    
```

## Se realiza un commit de los cambios.
```bash
"Se crea rama, ejercicio java": mensaje subido.
3de29e42f2dba93bc3559f6fc3ef5884f8716b48: numero del commit.
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




# Ejercicio 2.
 <div style="justify"> 

 ## Crear una nueva rama llamada *Ejercicio2-branch* y comprobando que se encuentra en la nueva rama.
 ```bash
 bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git checkout -b ejercicio2-branch
Cambiado a nueva rama 'ejercicio2-branch'
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git branch
  ejercicio1-branch
* ejercicio2-branch
  main
 ```

 ## Se crea un nuevo archivo ".java" con el nombre *Ejercicio2.java*.

```java
     public class Ejercicio2 {
     public static void main(String[] args) {
         System.out.println("Ejercicio 2 realizado.");
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
## Se elimina el archivo REAME.md sobrante y se hacen correcciones en el repositorio.
```bash
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ rm -rf Ejercicios-git-branch-nuevo/
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ mv ejercicio1.java Ejercicio1.java 
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git add .
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git commit -m "Se han efectuado correcciones en el repositorio"
[main 47532a3] Se han efectuado correcciones en el repositorio
 2 files changed, 1 deletion(-)
 rename ejercicio1.java => Ejercicio1.java (100%)
 delete mode 160000 Ejercicios-git-branch-nuevo

```

# Ejercicio 3.

## Crear una nueva rama llamada *Ejercicio3-branch* y comprobando que se encuentra en la nueva rama.

```bash
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git checkout -b ejercicio3-branch
Cambiado a nueva rama 'ejercicio3-branch'
bae2@jpexposito-VirtualBox:~/Ejercicios-git-branch-nuevo$ git branch
  ejercicio1-branch
  ejercicio2-branch
* ejercicio3-branch
  main
```
## Se crea un nuevo archivo ".java" con el nombre *ejercicio3.java*.

```java
public class Ejercicio3 {
    public static void main(String[] args) {
        System.out.println("Ejercicio 3 realizado.");
    }
}

```
