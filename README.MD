# Estación de Temperatura y Humedad con Arduino

> Un dispositivo simple y eficaz para monitorear la temperatura y la humedad ambiental en tiempo real, mostrando los datos en una pantalla LCD.

Este proyecto utiliza un sensor DHT22 para capturar mediciones precisas del ambiente y las presenta de manera clara en una pantalla I2C, sirviendo como una mini estación meteorológica personal o un sistema de monitoreo para proyectos que requieren control ambiental.

## ✨ Características Principales

*   **Monitoreo Dual**: Mide tanto la temperatura (°C) como la humedad relativa (%).
*   **Visualización Clara**: Muestra los datos de forma ordenada en una pantalla LCD de 16x2.
*   **Actualización Constante**: Refresca los valores cada 2 segundos para tener datos actualizados.
*   **Manejo de Errores**: Detecta si el sensor no está conectado correctamente y muestra un mensaje de error.
*   **Plataforma Abierta**: Basado en Arduino, una plataforma fácil de usar y modificar.

-----

## 🛠️ Componentes Necesarios

| Componente | Cantidad | Descripción |
| :--- | :---: | :--- |
| Arduino Uno | 1 | Placa microcontroladora principal. |
| Sensor de Temp. y Hum. DHT22 | 1 | Sensor principal para las mediciones. |
| Pantalla LCD I2C 16x2 | 1 | Muestra los datos obtenidos. |
| Protoboard (Placa de Pruebas) | 1 | Para montar el circuito sin soldar. |
| Cables Jumper (Macho-Hembra) | Varios | Para realizar las conexiones. |
| Resistencia de 10kΩ (Opcional) | 1 | Recomendada como pull-up para el pin de datos del DHT22. |


-----

## 🔌 Conexiones

Para ensamblar el proyecto, realiza las siguientes conexiones con cuidado.

### Conexión del Display LCD I2C

| Pin del LCD | Pin del Arduino Uno |
| :---: | :---: |
| GND | GND |
| VCC | 5V |
| SDA | A4 |
| SCL | A5 |

### Conexión del Sensor de Temperatura DHT22

| Pin del Sensor | Pin del Arduino Uno |
| :---: | :---: |
| VCC / + | 5V |
| DATA / OUT | **2** |
| GND / - | GND |

**Nota sobre la resistencia**: Para una mayor estabilidad en la lectura de datos, se recomienda conectar una resistencia de 10kΩ entre el pin de 5V y el pin de datos (Pin 2) del sensor.

## 📚 Librerías Necesarias

Para que el código compile correctamente, necesitas instalar las siguientes librerías desde el Gestor de Librerías del IDE de Arduino:

1.  **DHT sensor library** (por Adafruit)
2.  **LiquidCrystal I2C** (por Frank de Brabander)

## 👥 Autores y Agradecimientos

Este proyecto fue creado con fines educativos y de aprendizaje por:

*   [Felipe Colli](https://github.com/F-Patata2008) (F-Patata) 

## 📜 Licencia

Este proyecto es de dominio público o se puede licenciar bajo la **Licencia MIT**, que permite su libre uso, modificación y distribución.
