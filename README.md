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
  - `beautifulsoup4`
  - `urllib3`

---

## **Instalación**
1. Clona el repositorio:

   git clone https://github.com/Zuk4r1/VulnKit.git

   cd vulnkit
   
   chmod +x vulnkit.py

   pip install -r requirements.txt

---
## **Comandos de Ejecucion**
 * Escaneo de encabezados de seguridad:
  
  python vulnkit.py www.ejemplo.com --scan-headers

---
## **Ejecución de exploits:**

  python vulnkit.py www.ejemplo.com --exploit <tipo_de_exploit>

---
 ## **Tipos de exploits disponibles:**

 - **sqli:** Explota la inyección SQL.
 - **rce:** Prueba de ejecución remota de comandos.
 - **ssrf:** Evalúa SSRF.
 - **deserialization:** Prueba deserialización insegura.
 - **xss:** Explota secuencias de comandos entre sitios.
   
 ---
 ## **Ejemplo:**

  python vulnkit.py www.ejemplo.com --exploit sqli

---
## **Salida**

Los resultados se guardan en un archivo vulnerabilities_report.txt, que incluye:

* Vulnerabilidades detectadas.
* Detalles de los exploits utilizados.
* Comandos ejecutados.

---
## **Contribuciones**

¡Las contribuciones son bienvenidas! Si deseas agregar nuevas funciones o mejorar la herramienta, envía una solicitud de extracción o abre un problema en el repositorio.
