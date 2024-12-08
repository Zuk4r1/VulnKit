# **VulnKit - Escáner y Explotador de Vulnerabilidades**

VulnKit es una herramienta avanzada para la auditoría de seguridad y explotación de vulnerabilidades críticas. Diseñada para profesionales de la seguridad y entusiastas del pentesting, esta herramienta identifica y explota fallas en sistemas y aplicaciones web de manera ética y controlada.

# Características

Escaneo de encabezados de seguridad (CSP, X-Frame-Options, HTTPS, etc.).

### Identificación de vulnerabilidades críticas:

 * SQL Injection (SQLi)

 * Ejecución Remota de Comandos (RCE)

 * Server-Side Request Forgery (SSRF)

 * Deserialización Insegura

 * Cross-Site Scripting (XSS)

 * Falta de HTTPS

 * Ausencia de X-Frame-Options

 * Inyección LDAP

 * Directory Traversal (DT)

 * Cross-Site Request Forgery (CSRF)

 * SSL/TLS Vulnerabilities

 * Búsqueda genérica de vulnerabilidades no cubiertas por exploits predefinidos.
  
 * Ejecución de exploits personalizados para probar la seguridad del objetivo.

 * Reportes detallados en formato de tabla, guardados automáticamente en un archivo .txt.

# Requerimientos

 * Python 3.8+

   **Librerías externas (instalar con pip):**

 * requests

 * argparse

 * beautifulsoup4

 * urllib3

# Instalación

Clona el repositorio:

  git clone https://github.com/Zuk4r1/VulnKit.git

* cd vulnkit

* chmod +x vulnkit.py

* pip install -r requirements.txt

# Comandos de Ejecución

 * **Escaneo de encabezados de seguridad:**

python vulnkit.py www.ejemplo.com --scan-headers

 * **Ejecución de exploits específicos:**

python vulnkit.py www.ejemplo.com --exploit <tipo_de_exploit>

 * **Escaneo de vulnerabilidades genéricas:**

python vulnkit.py www.ejemplo.com --scan-generic

 * **Ejecución de todos los exploits disponibles:**

python vulnkit.py www.ejemplo.com --scan-all

# Tipos de Exploits Disponibles

**sqli:** Explota la inyección SQL.

**rce:** Prueba de ejecución remota de comandos.

**ssrf:** Evalúa SSRF.

**deserialization:** Prueba deserialización insegura.

**xss:** Explota secuencias de comandos entre sitios.

**ldap_injection:** Detecta y explota inyecciones LDAP.

**dt:** Realiza pruebas de directory traversal.

**csrf:** Evalúa vulnerabilidades de Cross-Site Request Forgery.

**x_frame:** Detecta la ausencia de X-Frame-Options.

**https:** Evalúa la ausencia de HTTPS.

# Ejemplo de Ejecución

* **Escanear encabezados de seguridad:**

python vulnkit.py www.ejemplo.com --scan-headers

* **Ejecutar un exploit específico (ejemplo: SQLi):**

python vulnkit.py www.ejemplo.com --exploit sqli

* **Escaneo genérico:**

python vulnkit.py www.ejemplo.com --scan-generic

* **Ejecutar todos los exploits disponibles:**

python vulnkit.py www.ejemplo.com --scan-all

# Salida

Los resultados se guardan en un archivo **Report_<fecha_hora>.txt**, que incluye:

* Vulnerabilidades detectadas.

* Detalles de los exploits utilizados.

* Comandos ejecutados.

El archivo se genera en formato de tabla con descripciones claras, versiones afectadas y detalles técnicos de cada vulnerabilidad encontrada.

# Contribuciones

¡Las contribuciones son bienvenidas! Si deseas agregar nuevas funciones o mejorar la herramienta, envía una solicitud de extracción o abre un problema en el repositorio.
