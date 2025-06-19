# 🛡️**VulnKit - Escáner y Explotador de Vulnerabilidades**

**VulnKit** es una herramienta avanzada para la auditoría de seguridad y explotación de vulnerabilidades críticas. Diseñada para profesionales de la seguridad y entusiastas del pentesting, esta herramienta identifica y explota fallas en sistemas y aplicaciones web de manera ética y controlada.

# ⚙️ Características

Escaneo de encabezados de seguridad: Detecta encabezados críticos ausentes o mal configurados, como Content-Security-Policy, X-Frame-Options, Strict-Transport-Security, y más.

**Identificación de vulnerabilidades críticas, como:**

* Inyección SQL (SQLi)

* Ejecución Remota de Comandos (RCE)

* Server-Side Request Forgery (SSRF)

* Deserialización insegura

* Cross-Site Scripting (XSS)

* Falta de HTTPS

* Inyección LDAP

* Directory Traversal (DT)

* Cross-Site Request Forgery (CSRF)

* Redirecciones inseguras (Open Redirect)

* Inyección de Entidades Externas XML (XXE)

* Subida insegura de archivos

* Detección de vulnerabilidades modernas como Log4Shell o ProxyLogon

**Escaneo genérico de vulnerabilidades:** Evalúa posibles fallas que no estén cubiertas por exploits específicos.

**Ejecución de exploits personalizados:** Compatible con una amplia gama de exploits preconfigurados.

**Exploración web (Spidering):** Rastrea enlaces y formularios en aplicaciones web.

**Reportes automáticos:** Genera informes claros en formato .txt con detalles de las vulnerabilidades detectadas.

## 🔥 Mejoras Avanzadas

1. **Escaneo avanzado de puertos**: Multithreading para alta velocidad y detección de servicios activos.
2. **Detección avanzada de tecnologías**: Analiza headers, frameworks JS, CMS, archivos `robots.txt`, `sitemap.xml`, y más.
3. **Detección de WAFs y mecanismos de protección**: Análisis de headers, cookies, detección de firmas conocidas, captchas, respuestas anómalas.
4. **Escaneo agresivo de subdominios**: Uso de hilos y diccionarios extendidos.
5. **Payloads polimórficos y avanzados**: Cientos de vectores para SQLi, XSS, RCE, SSRF y más.
6. **Soporte de exploits modulares**: Carga dinámica de scripts externos.
7. **Generación de reportes JSON estructurados**: Perfecto para análisis automatizado y pipelines.
8. **Soporte para proxies y configuración de hilos**: Personaliza cada escaneo a tu entorno.
9. **Logging avanzado**: Guarda logs detallados de cada escaneo, resultado y fallo.
10. **Detección de paneles administrativos y puntos de carga de archivos**.
11. **Evasión y antifiltro**: Uso de User-Agents aleatorios, cambios de headers, codificaciones, y más.

# 📦 Requerimientos:
```
Python: 3.8 o superior.
```

* Dependencias **requests, argparse, beautifulsoup4, urllib3, dnspython, nmap,** entre otras.

# 🧰 Librerías externas (instalar con pip):
```
pip install -r requirements.txt
```

# 📥 Instalación

* Clona el repositorio:
```
git clone https://github.com/Zuk4r1/VulnKit.git
```
# 📁 Acedemos al Directorio:
```
cd vulnkit
```
# 🔐 Le damos permisos de escritura, lectura y ejecucion.
```
chmod +x vulnkit.py
```

# 🧪 Comandos de Ejecución

* Escaneo de encabezados de seguridad:
```
python vulnkit.py www.ejemplo.com --scan-headers
```

# 🎯 Ejecución de exploits específicos:
```
python vulnkit.py www.ejemplo.com --exploit <tipo_de_exploit>
```

# 🔍 Escaneo de vulnerabilidades genéricas:
```
python vulnkit.py www.ejemplo.com --scan-generico
```

# 💣 Ejecución de todos los exploits disponibles:
```
python vulnkit.py www.ejemplo.com --scan-all
```

# 🧠 Escanear encabezados de seguridad:
```
python vulnkit.py www.ejemplo.com --scan-headers
```
# 🆘 Menu de ayuda
Muestra todas las opciones y funciones que tiene la herramienta.
```
python vulnkit.py -h
```

# 🧨 Tipos de Exploits Disponibles

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

# 📤 Salida

* Los resultados se guardan en un archivo Report_<fecha_hora>.txt, que incluye:

* Vulnerabilidades detectadas.

* Detalles técnicos sobre cada vulnerabilidad encontrada.

* Comandos ejecutados.

* El archivo se genera en formato de tabla con descripciones claras, versiones afectadas y detalles técnicos.

# 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si deseas agregar nuevas funciones o mejorar la herramienta, envía una solicitud de extracción o abre un problema en el repositorio. Este texto actualizado refleja todas las mejoras implementadas en VulnKit, asegurando que los usuarios estén informados sobre las capacidades avanzadas y las nuevas características disponibles en la herramienta.

## 🎁 ¡Apoya el proyecto!

Si esta herramienta te ha sido útil, puedes apoyar su desarrollo con una donación:

☕ [Buy Me a Coffee](https://buymeacoffee.com/investigacq)

💸 [PayPal](https://www.paypal.com/paypalme/babiloniaetica)

# 🧠 Autor

Created with ❤️ by [@Zuk4r1](https://github.com/Zuk4r1). – defensor del hacking ético y la investigación digital.

## ⚖️ LICENCIA
Este proyecto está licenciado bajo la licencia **MIT**. Consulte el archivo [`LICENCIA`](https://github.com/Zuk4r1/VulnKit/blob/main/LICENSE) para más detalles.

## ¡Feliz hackeo! 🎯
