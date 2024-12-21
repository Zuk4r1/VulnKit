# **VulnKit - Escáner y Explotador de Vulnerabilidades**

VulnKit es una herramienta avanzada para la auditoría de seguridad y explotación de vulnerabilidades críticas. Diseñada para profesionales de la seguridad y entusiastas del pentesting, esta herramienta identifica y explota fallas en sistemas y aplicaciones web de manera ética y controlada.

# Características

* Escaneo de encabezados de seguridad: Verifica la presencia de encabezados críticos como Content-Security-Policy, X-Frame-Options, HTTPS, Strict-Transport-Security, y más.

* Identificación de vulnerabilidades críticas:

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

* Open Redirect

* XML External Entity Injection (XXE)
  
**Búsqueda genérica de vulnerabilidades:** Escanea vulnerabilidades no cubiertas por exploits predefinidos.

**Ejecución de exploits personalizados:** Permite probar la seguridad del objetivo con exploits específicos.

**Reportes detallados:**  Genera reportes en formato de tabla que se guardan automáticamente en un archivo .txt, incluyendo vulnerabilidades detectadas, detalles técnicos, versiones afectadas y comandos utilizados.

# Requerimientos

* **Python 3.8+**

# Librerías externas (instalar con pip):

**pip install -r requirements.txt**

* requests

* argparse

* beautifulsoup4

* urllib3

* dns-python

# Instalación

* Clona el repositorio:

**git clone https://github.com/Zuk4r1/VulnKit.git**

**cd vulnkit**

**chmod +x vulnkit.py**

# Comandos de Ejecución

* Escaneo de encabezados de seguridad:

**python vulnkit.py www.ejemplo.com --scan-headers**

# Ejecución de exploits específicos:

**python vulnkit.py www.ejemplo.com --exploit <tipo_de_exploit>**

# Escaneo de vulnerabilidades genéricas:

**python vulnkit.py www.ejemplo.com --scan-generic**

# Ejecución de todos los exploits disponibles:

**python vulnkit.py www.ejemplo.com --scan-all**

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

**open_redirect:** Evalúa redirecciones inseguras.

**xxe:** Evalúa inyecciones XML externas.

# Ejemplo de Ejecución

* Escanear encabezados de seguridad:

**python vulnkit.py www.ejemplo.com --scan-headers**

# Ejecutar un exploit específico (ejemplo: SQLi):

**python vulnkit.py www.ejemplo.com --exploit sqli**

# Escaneo genérico:

**python vulnkit.py www.ejemplo.com --scan-generic**

# Ejecutar todos los exploits disponibles:

**python vulnkit.py www.ejemplo.com --scan-all**

# Salida

* Los resultados se guardan en un archivo Report_<fecha_hora>.txt, que incluye:

* Vulnerabilidades detectadas.

* Detalles técnicos sobre cada vulnerabilidad encontrada.

* Comandos ejecutados.

* El archivo se genera en formato de tabla con descripciones claras, versiones afectadas y detalles técnicos.

# Contribuciones

¡Las contribuciones son bienvenidas! Si deseas agregar nuevas funciones o mejorar la herramienta, envía una solicitud de extracción o abre un problema en el repositorio. Este texto actualizado refleja todas las mejoras implementadas en VulnKit, asegurando que los usuarios estén informados sobre las capacidades avanzadas y las nuevas características disponibles en la herramienta.
