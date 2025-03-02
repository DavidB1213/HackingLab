# 🏴‍☠️ DarkHole: 2 - Documentación de Explotación

> **Fuente:** [VulnHub - DarkHole: 2](https://www.vulnhub.com/entry/darkhole-2,740/)  
> **Dificultad:** Media  
> **IP de la máquina:** `192.168.1.105`  

---

## 🔎 1. Reconocimiento (Escaneo y Enumeración)

### **Escaneo de puertos con Nmap**
```bash
nmap -sC -sV -p- 192.168.1.105 -oN darkhole2_nmap.txt
```
📌 **Servicios detectados:**
```
22/tcp   open  ssh         OpenSSH 7.6p1 Ubuntu 4ubuntu0.3
80/tcp   open  http        Apache httpd 2.4.29
3306/tcp open  mysql       MySQL 5.7.33
```
**Análisis:**
- Puerto **80** (HTTP) → Página web activa, posible vector de ataque.
- Puerto **3306** (MySQL) → Podría contener credenciales vulnerables.
