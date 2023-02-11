# git_1_daw

### otros comandos de interes

git status
git branch

##ESTO ES UN REPOSITORIO PARA LA TAREA 3 DE ENTORNOS DE DESARROLLO

1) git clone/// clonar el repositorio creado
2) git add para añadir el archivo al seguimiento de git
3) git commit -m "comentario"
4) git push para subir los cambios al repositorio

## TABLA COMPAÑEROS

| NOMBRE | GITHUB |
|--------|--------|
|Jose Manuel|[github](https://github.com/jbenalb)|
|Alejandro|[github](https://github.com/asecval543)|
|Abraham|[github](https://github.com/arodmor789)|
|Pablo|[github](https://github.com/pamadob)|

## CREANDO EL .GITIGNORE
touch privado.txt
mkdir privada
nano .gitignore
git add .gitignore
git commit -m "añadido .gitignore"
git push

## CREANDO LA TAG Y EL ARCHIVO 1.TXT

 touch 1.txt
 git add 1.txt
 git tag v.0.1
 git commit -am "añadido 1.txt y el tag v.0.1"
 git push 

##COMANDOS REALIZACIÓN TABLA

nano README.md
git commit -am "añadida tabla compañeros"
git push

## CREANDO LA RAMA V0.2 Y HACIENDO UN PUSH

  git branch v0.2
  git checkout v0.2
  touch 2.txt
  git add 2.txt
  git commit -m "añadido el archivo 2.txt a la rama v0.2"
  git push -u origin v0.2

## MERGE SIN CONFLICTO

 git checkout main
 git branch
 git merge v0.2

## MERGE CON CONFLICTO

 nano 1.txt
  git add 1.txt
  git commit -m "Añadido hola en rama main"
  git checkout v0.2
  nano 1.txt
  git add 1.txt
  git commit -m "Añadido Adios en la rama v0.2"
  git checkout main
  git merge v0.2
  nano 1.txt
  git commit -am "conflicto resuelto en 1.txt"
  git push

## CREANDO TAG V0.2, ELIMINANO LA RAMA Y ENSEÑANDO LOS CAMBIOS

   git tag v0.2
   git checkout v0.2/// subir lo que quedaba en la rama al repositorio local, con -D fuerzas a borrar la rama aunque tengas cambios pendientes.
   git push
   git checkout main
   git branch -d v0.2
   git log --graph

## CREANDO EL ARCHIVO equipo.md

  touch equipo.md
  nano equipo.md
  git add equipo.md
  git commit -m "añadido equipo.md"
  git push






