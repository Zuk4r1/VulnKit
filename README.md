# VulnKit - Escáner y Explotador de Vulnerabilidades

**VulnKit** es una herramienta avanzada para la auditoría de seguridad y explotación de vulnerabilidades críticas. Diseñada para profesionales de la seguridad y entusiastas del pentesting, esta herramienta identifica y explota fallas en sistemas y aplicaciones web de manera ética y controlada.

---

## **Características**
- Escaneo de encabezados de seguridad (CSP, X-Frame-Options, etc.).
- Identificación de vulnerabilidades críticas:
  - **SQL Injection (SQLi)**
  - **Ejecución Remota de Comandos (RCE)**
  - **Server-Side Request Forgery (SSRF)**
  - **Deserialización Insegura**
  - **Cross-Site Scripting (XSS)**
- Ejecución de exploits personalizados para probar la seguridad del objetivo.
- Reportes detallados en formato de tabla, guardados automáticamente en un archivo `.txt`.

---

## **Requerimientos**
- **Python 3.8+**
- Librerías externas (instalar con `pip`):
  - `requests`
  - `argparse`
  - `prettytable`

---

## **Instalación**
1. Clona el repositorio:
   ```bash
   git clone https://github.com/Zuk4r1/VulnKit.git
   cd vulnkit
   chmod +x vulnkit.py
   pip install -r requirements.txt

