# 🛠️ DarkHole: 2 - Documentación de Explotación

> **Categoría:** Máquina Virtual de Prueba  
> **Dificultad:** Fácil  
> **IP:** `192.168.1.100` 

## 🔎 1. Reconocimiento (Escaneo y Enumeración)

Ejecutamos un escaneo con Nmap para identificar los servicios activos:

```bash
nmap -sC -sV -p- 192.168.1.100 -oN vulnbox_nmap.txt
```
### **Resultados del escaneo**
```
PORT     STATE SERVICE     VERSION
22/tcp   open  ssh         OpenSSH 7.2p2 Ubuntu 4ubuntu2.8
80/tcp   open  http        Apache httpd 2.4.18
```

**Análisis:**
- El puerto **22** (SSH) está abierto → Posible ataque de fuerza bruta o exploits conocidos.
- El puerto **80** (HTTP) está abierto → Puede haber una vulnerabilidad en la web.

---