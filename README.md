### PACHA: Software para la Alineación de Grafos Químicos

**Descripción:**
PACHA es una herramienta de software para alinear grafos químicos.

**Uso:**
- Para utilizar PACHA, dirígete al directorio 'pacha/src', ejecuta 'make' y luego corre './pacha --input_file=string --output_file=string [opciones] ...'.
- Las opciones incluyen:
  - -i, --input_file: Nombre del archivo de entrada (cadena)
  - -o, --output_file: Nombre del archivo de salida (cadena)
  - -d, --dist: Distancia máxima para calcular características de vértices (entero largo sin signo [=5])
  - -k, --topk: Número de alineaciones a partir de pares de vértices con las mejores puntuaciones coincidentes (entero largo sin signo [=10])
  - -n, --num_threads: Número de hilos (entero largo sin signo [=1])
  - -t, --threshold: Umbral (flotante [=0])
  - -c, --inter_cuts: Número máximo de cortes intermoleculares (entero largo sin signo [=100000000])
  - -a, --intra_cuts: Número máximo de cortes intramoleculares (entero largo sin signo [=100000000])
  - -?, --help: Imprimir este mensaje

**Requisitos:**
- Compilador GNU C++ (Versiones superiores son preferibles para multi-hilos).

**Instalación:**
- Para instalar PACHA, ve al directorio 'pacha/src' y ejecuta 'make'.

**Licencia:** Licencia MIT
