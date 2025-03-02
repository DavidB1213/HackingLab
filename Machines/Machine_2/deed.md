# 🛠️ DarkHole: 2 - Documentación de Explotación

> **Categoría:** Máquina Virtual de Prueba  
> **Dificultad:** Fácil  
> **IP:** `192.168.1.100` 

## 🔎 1. Reconocimiento (Escaneo y Enumeración)

Ejecutamos un escaneo con Nmap para identificar los servicios activos:

```bash
nmap -sC -sV -p- 192.168.1.100 -oN vulnbox_nmap.txt
```