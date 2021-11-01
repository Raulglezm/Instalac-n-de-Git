# Instalación de Git
![image](https://user-images.githubusercontent.com/91153605/139741290-b476f342-9c39-42fb-85a7-4ec4f7e98dd6.png)

## Paso 1
![image](https://user-images.githubusercontent.com/91153605/139737145-bedf2267-c7ac-4d66-8f1f-b547cc9a69d5.png)

```bash 
git --version
```
Con este comando comprobaremos si tenemos instalado Git en nuestro sistema y si es así podremos ver de qué versión se trata

## Paso 2
![image](https://user-images.githubusercontent.com/91153605/139737319-7366079c-3e3a-4517-9a28-f24f1cfe2b5b.png)
```bash
sudo apt update
```
Si no lo teníamos instalado deberemos usar este comando para actualizar los paquetes
## Paso 3
![image](https://user-images.githubusercontent.com/91153605/139737414-e9d908e4-d59c-4164-9110-9f74ee2f4a7b.png)
```bash
sudo apt install git
```
Una vez instalado comprobaremos que está bien instalado con el comando ```git --version ```
## Paso 4
![image](https://user-images.githubusercontent.com/91153605/139737566-6fd84aa9-5822-4d8f-9f24-d8db80e62604.png)

```bash
sudo apt update
sudo apt install libz-dev libssl-dev libcurl4-gnutls-dev libexpat1-dev gettext cmake gcc
```
Con estos comandos instalaremos dependencias necesarias para modificar Git

## Paso 5
![image](https://user-images.githubusercontent.com/91153605/139742270-4b312ac1-c927-4577-8e13-05d30aa1cc60.png)
Nos colocaremos en el directorio tmp con los comandos 
```bash
mkdir tmp
cd /tmp
```
Y posteriormente descargaremos la vesion más reciente de git.
```bash 
curl -o git.tar.gz https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.29.3.tar.gz
```
Si este comando te da problemas debes instalar curl con el comando ```sudo apt install curl```

## Paso 6
![image](https://user-images.githubusercontent.com/91153605/139742937-ec6a5881-3dcd-4843-8ff1-ea053ca14100.png)

```bash
tar -zxf git.tar.gz
```
Para descomprimir el paquete.

## Paso 7
![image](https://user-images.githubusercontent.com/91153605/139745032-707b47be-7de2-4cbf-a3e2-d23e061bb612.png)
No colocamos en el directorio ```git-*```

## Paso 8 
![image](https://user-images.githubusercontent.com/91153605/139745209-91a62e1b-5af3-46e6-b3ba-6dbe74b7fc65.png)
```bash 
make prefix=/usr/local all
sudo make prefix=/usr/local install
```
Con estos comandos crearemos e instalaremos el paquete

## Paso 9
![image](https://user-images.githubusercontent.com/91153605/139745626-a96169ce-c3c4-4ffd-b5bb-cd9469fb9d0a.png)

Para finalizar introduciremos el comando ```exec bash``` y por último ```git --version``` comprobando que la versión es la deseada






