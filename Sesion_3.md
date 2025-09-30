Documentación del proyecto — Esqueleto Tkinter (6 ventanas) Autor: Generado por ChatGPT (developer profesional de Python) Fecha: 2025-09-26 Descripción: Este documento explica el funcionamiento de un proyecto de aplicación de escritorio en Python usando Tkinter. El proyecto consta de seis módulos principales que representan la ventana principal y cinco ventanas secundarias con diferentes funcionalidades.

Estructura del proyecto / (raíz del proyecto) ├─ src/app/ │ ├─ main.py # Ventana principal │ ├─ win_home.py # Ventana de bienvenida │ ├─ win_form.py # Ventana con formulario │ ├─ win_list.py # Ventana con lista y CRUD │ ├─ win_table.py # Ventana con tabla Treeview │ └─ win_canvas.py # Ventana con canvas para dibujar ├─ data/sample.csv # Datos de ejemplo para la tabla ├─ docs/ # Documentación del proyecto └─ .vscode/launch.json Propósito general El proyecto tiene como objetivo demostrar el uso de Tkinter para crear aplicaciones de escritorio con múltiples ventanas, permitiendo: • Navegación desde la ventana principal. • Formularios con validación y guardado en archivos. • Operaciones CRUD en listas. • Visualización de datos CSV en tablas. • Dibujo gráfico simple en un canvas.
Documentación de módulos 2.1 main.py Propósito: Es el punto de entrada de la aplicación. Muestra la ventana principal con botones para abrir cada una de las ventanas secundarias. Flujo de la aplicación:
Se crea la ventana principal con Tk().
Se configura el título y dimensiones.
Se añade un frame principal con padding.
Se crean botones para cada ventana secundaria (Home, Form, List, Table, Canvas) y un botón de salida.
Se ejecuta root.mainloop() para iniciar la aplicación. 2.2 win_home.py Propósito: Ventana de bienvenida que permite mostrar mensajes de información al usuario. Flujo:
Se crea una ventana Toplevel que depende de la ventana principal.
Se añade un frame con padding.
Se muestran etiquetas con texto de bienvenida.
Se añade un botón que despliega un mensaje usando messagebox.showinfo().
Se añade un botón de cierre para destruir la ventana. Notas: Ventana simple que demuestra interactividad básica. 2.3 win_form.py Propósito: Proporciona un formulario para capturar el nombre y la edad del usuario y guardar la información en un archivo de texto. Flujo:
Crear ventana Toplevel con frame.
Añadir labels y entradas (Entry) para Nombre y Edad.
Botón "Guardar" que llama a validar_y_guardar(): o Valida que el nombre no esté vacío. o Valida que la edad sea un número entero. o Abre un filedialog para elegir la ubicación del archivo. o Escribe los datos en un archivo .txt.
Botón de cierre para destruir la ventana. Notas: Validación robusta de entradas y feedback con messagebox. 2.4 win_list.py Propósito: Ventana para gestionar una lista de elementos con operaciones CRUD básicas. Flujo:
Crear ventana Toplevel con frame.
Añadir un Listbox y entrada de texto para nuevo elemento.
Botón "Agregar" que inserta texto en la lista si no está vacío.
Botón "Eliminar seleccionado" que elimina el elemento marcado.
Botón "Limpiar" que elimina todos los elementos de la lista.
Botón de cierre para destruir la ventana. Notas: Permite al usuario interactuar directamente con la lista y ver cambios en tiempo real. 2.5 win_table.py Propósito: Visualización de datos tabulares desde un archivo CSV usando ttk.Treeview. Flujo:
Crear ventana Toplevel con frame.
Configurar columnas del Treeview y encabezados.
Verificar que el archivo sample.csv existe.
Leer los datos del CSV con csv.DictReader.
Insertar filas en el Treeview.
Botón de cierre para destruir la ventana. Notas: Permite mostrar datos de forma ordenada y es fácil de expandir para manejar más columnas o datos. 2.6 win_canvas.py Propósito: Ventana con un canvas donde se dibujan formas básicas como rectángulos, óvalos, líneas y texto. Flujo:
Crear ventana Toplevel con frame.
Añadir un Canvas con dimensiones y color de fondo.
Dibujar ejemplos de rectángulo, óvalo, línea y texto.
Botón de cierre para destruir la ventana. Notas: Permite experimentar con gráficos en Tkinter y es base para dibujos más complejos.
Guía de uso
Ejecutar el proyecto desde main.py.
La ventana principal muestra botones numerados para abrir cada ventana.
Cada ventana secundaria se puede cerrar independientemente.
Para guardar datos en el formulario, seleccionar una ubicación en el diálogo de archivo.
Flujo de navegación Ventana Principal ├─ Home / Bienvenida ├─ Formulario ├─ Lista (CRUD) ├─ Tabla (Treeview) └─ Canvas (Dibujo)
Dependencias • Python 3.10+. • Tkinter incluido con Python. • Opcional: csv y pathlib para manejo de archivos.
Buenas prácticas aplicadas • Modularización: Cada ventana en un módulo independiente. • Uso de Toplevel para ventanas secundarias. • Validaciones de entradas y feedback con messagebox. • Separación de UI y lógica mínima para futuras expansiones.
