Shock_nrf52
==================
 
 Ce projet reprend celui fournis par Nordic Semiconductor "ble_app_uart__saadc_timer_driven__scan_mode" en ajoutant les fonctionnalités spécifiques pour le Shock d'Innovalab. 
 
 - Echantillonnage avec un ADC
 - Communication entre Android et nRF52 en BLE/UART
 - Gestion des envois bluetooth par paquets
 
  Les seules modifications majeures effectuées sont dans le fichier main.c, d'autres fichiers ont été modifiés mais uniquement pour des paramètrages divers. 

La version compatible avec notre carte nRF52 est pca10040/s132/arm5_no_packs/ble_app_uart_s132_pca10040.uvprojx

Version originale de Nordic Semiconductor
==================
 
This project contains a code example that shows nrf52 SAADC scan mode and how to integrate SAADC with softdevice.
 
Requirements
------------
- nRF5 SDK version 11.0.0
- nRF52-DK
- Softdevice S132 2.0.x

To compile it, clone the repository in the \nRF5_SDK_11.0.0_89a8197\examples\peripheral\ folder.  


Documentation
-----------------
- Perhipheral: nRF52 SAADC
- Compatibility: nRF52 rev 1, nRF5 SDK 11.0.0
- Softdevice used: S132 2.0.1

This SAADC example samples on 4 different input pins, and enables scan mode to do that. It is otherwise an offspring from the standard ble_app_uart example available in nRF5 SDK 11.0.0

- Transmits SAADC output to hardware UART and over BLE via Nordic UART Servive (NUS).
- Info on NUS -> http://infocenter.nordicsemi.com/topic/com.nordic.infocenter.sdk5.v11.0.0/ble_sdk_app_nus_eval.html?cp=5_0_0_4_2_2_18
- Info on hardware UART settings -> http://infocenter.nordicsemi.com/topic/com.nordic.infocenter.sdk5.v11.0.0/uart_example.html?cp=5_0_0_4_5_33

About this project
------------------
This application is one of several applications that has been built by the support team at Nordic Semiconductor, as a demo of some particular feature or use case. It has not necessarily been thoroughly tested, so there might be unknown issues. It is hence provided as-is, without any warranty. 

However, in the hope that it still may be useful also for others than the ones we initially wrote it for, we've chosen to distribute it here on GitHub. 

The application is built to be used with the official nRF5 SDK, that can be downloaded from http://developer.nordicsemi.com/

Please post any questions about this project on https://devzone.nordicsemi.com.
