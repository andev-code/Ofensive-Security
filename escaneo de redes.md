## Detalles sobre Escaneo de Redes en eJPT

### 1. Descubrimiento de Dispositivos:
   - **Herramientas Utilizadas:** Una herramienta clave para el descubrimiento de dispositivos es Nmap (Network Mapper). Nmap permite realizar un escaneo de la red para descubrir hosts activos, sus direcciones IP y los servicios que están en ejecución.
     ```bash
     nmap -sn <rango de IP>
     ```
   - **Identificación de Servicios Abiertos:** Nmap también es útil para identificar servicios abiertos en los dispositivos descubiertos. Esto se realiza mediante un escaneo de puertos.
     ```bash
     nmap -p- <dirección IP>
     ```

### 2. Mapeo de la Topología:
   - **Análisis de Redes:** Se realiza un análisis detallado de la estructura de la red. Esto implica comprender la disposición física y lógica de los dispositivos, así como la interconexión entre ellos.
   - **Diagramación de Redes:** Dependiendo de la situación, puede ser necesario crear diagramas para representar visualmente la topología de la red. Herramientas como draw.io o Lucidchart pueden ser útiles para esta tarea.

### 3. Enumeración de Recursos:
   - **Identificación de Recursos Compartidos:** Se busca descubrir recursos compartidos, como impresoras o carpetas compartidas en la red. Esto puede realizarse mediante el escaneo de servicios específicos.
     ```bash
     nmap --script smb-enum-shares -p 445 <dirección IP>
     ```
   - **Enumeración de Hosts y Puertos:** Además del escaneo inicial, se puede realizar un escaneo más detallado para enumerar hosts y puertos específicos.
     ```bash
     nmap -p 80,443,21 <dirección IP>
     ```

### Prácticas Recomendadas para el Escaneo de Redes:
1. **Entrenamiento Práctico:** Utiliza entornos de laboratorio virtual para practicar el escaneo de redes en situaciones controladas.
2. **Comprensión de Contexto:** Antes de realizar un escaneo, comprende el contexto de la red, incluyendo sus límites y cualquier política de seguridad existente.
3. **Documentación Detallada:** Documenta cuidadosamente los resultados de tus escaneos, incluyendo direcciones IP, servicios encontrados y cualquier hallazgo relevante.

El escaneo de redes es una habilidad esencial en ciberseguridad, ya que sienta las bases para identificar posibles vulnerabilidades y puntos de entrada en una infraestructura. Estas técnicas, combinadas con un enfoque ético, son fundamentales para el éxito en el hacking ético.
