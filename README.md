# Genomica-evolutiva_Code01
Herramienta para descargar SRA toolkit
## PASO 1: 
Acceder a la terminal.
## PASO 2: 
# Seguir las instrucciones para la descarga en el siguiente link, teniendo en cuenta que se debe instalar para Linux:
# https://github.com/ncbi/sra-tools/wiki/01.-Downloading-SRA-Toolkit
## PASO 3:
# Descargar el archivo comprimido usando:
wget https://ftp-trace.ncbi.nlm.nih.gov/sra/sdk/3.1.1/sratoolkit.3.1.1-ubuntu64.tar.gz -O /ruta/deseada/stk.tar.gz
# wget: comando para descargar archivos desde la web.
# -O stk.tar.gz: -O hace referencia al output y stk.tar.gz es el nombre con el que se guardará el archivo. La ruta deseada es la ruta donde se prefiera guardar el archivo
## PASO 4: 
# Cambiar los permisos para que el archivo sea ejecutable. Se debe especificar la ruta. 
chmod 777 /ruta/deseada/stk.tar.gz
## PASO 5: 
# Agrega el directorio bin del SRA Toolkit al PATH temporalmente, para que se puedan ejecutar los programas de SRA Toolkit desde cualquier ubicación en la terminal sin necesidad de especificar su ruta completa.
export PATH=$PATH:$PWD/ ruta/deseada/sratoolkit.3.0.10-ubuntu64/bin
# $PATH: mantiene las rutas actuales que ya están en PATH.
# $PWD: es una variable que contiene la ruta completa del directorio actual (donde ejecutaste el comando).
# ruta/deseada/sratoolkit.3.0.10-ubuntu64/bin: Es la subcarpeta que contiene los ejecutables del SRA Toolkit.
# Finalmente el sistema podrá reconocer las herramientas de SRA Toolkit que están en la carpeta bin del paquete descomprimido.


