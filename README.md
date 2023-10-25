# DicciFusion por F3nix
![WhatsApp Image 2023-10-25 at 12 37 21](https://github.com/f3nixuy/DicciFusion/assets/50671074/f96e1b45-66b4-4f31-afb4-de4e1c09e6f9)


"ProcesaTextos y Más" es una herramienta multifuncional que procesa texto, crea superdiccionarios, escanea redes, mide la velocidad de Internet y obtiene información de IP. Una solución versátil para tareas diversas.

Este programa es una interfaz gráfica desarrollada en Python con la biblioteca Tkinter que combina varias funcionalidades relacionadas con el procesamiento de archivos de texto, así como una funcionalidad adicional para la creación de un superdiccionario a partir de varios diccionarios. Además, ofrece la capacidad de realizar escaneos de red mediante ARP, medir la velocidad de Internet y obtener la dirección IP del usuario para abrir Google Maps. Aquí está una descripción de sus principales características y cómo funciona:

1. **Procesamiento de archivos de texto y creación de superdiccionario:**
   - El programa permite al usuario seleccionar archivos de texto (archivos con extensión .txt) a través del botón "Agregar Archivo".
   - Las palabras únicas en los archivos seleccionados se extraen y se almacenan en un archivo llamado "resultado.txt". Esto se hace a través del botón "Generar Resultado".
   - Adicionalmente, el programa ofrece la opción de agregar varios diccionarios de palabras y crear un solo "superdiccionario" que podría utilizarse, por ejemplo, en ataques de fuerza bruta.

2. **Escaneo ARP:**
   - El programa realiza un escaneo de la red local mediante ARP (Address Resolution Protocol) al presionar el botón "Escanear ARP".
   - Muestra el resultado del escaneo en la etiqueta de resultados.

3. **Medición de la velocidad de Internet:**
   - Al hacer clic en el botón "Medir Velocidad de Internet", el programa utiliza la biblioteca `speedtest` para medir la velocidad de descarga, subida y el ping.
   - Los resultados se muestran en la etiqueta de resultados.

4. **Obtener la dirección IP y abrir Google Maps:**
   - Al hacer clic en "Obtener IP y Abrir Mapa", el programa utiliza la biblioteca `requests` para obtener la dirección IP del usuario a través del servicio "ipinfo.io".
   - Luego, si se obtiene la dirección IP, se utiliza la información de ubicación para abrir Google Maps en el navegador web con la ubicación aproximada del usuario.

Las librerías que debes tener instaladas para que el programa funcione son:
- `tkinter`: Para la creación de la interfaz gráfica.
- `subprocess`: Para ejecutar comandos del sistema operativo.
- `speedtest`: Para medir la velocidad de Internet.
- `requests`: Para realizar solicitudes a servicios web y obtener la dirección IP.

El programa crea una ventana principal con botones para ejecutar las diferentes funcionalidades. Los resultados se muestran en una etiqueta en la ventana. Al finalizar la descripción del programa, se ejecuta la interfaz gráfica con `ventana.mainloop()`, lo que permite al usuario interactuar con las diferentes funciones.
