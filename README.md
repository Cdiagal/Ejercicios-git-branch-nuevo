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

## Se crea un nuevo archivo ".java" con el nombre *ejercicio1.java*.

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




