# Proyecto-integrador-T.A.P.
📘 **Proyecto Integrador T.A.P. – Unidad 1**  
💻 Desarrollo de Formulario Web con Validaciones en Flet  

---

#  Proyecto Integrador 

El presente repositorio documenta el desarrollo del **Proyecto Integrador correspondiente a la Unidad 1**, enfocado en la construcción de una interfaz gráfica interactiva mediante el uso del framework Flet en el lenguaje de programación Python.

Este proyecto tiene como finalidad integrar los conocimientos fundamentales adquiridos durante la unidad, tales como:

- Diseño de interfaces gráficas
- Validación y control de datos
- Programación orientada a eventos
- Manejo de estructuras condicionales
- Aplicación de expresiones regulares
- Organización visual de componentes

El trabajo desarrollado demuestra la capacidad de diseñar un sistema funcional que interactúe con el usuario, valide información en tiempo real y garantice la integridad de los datos ingresados..

---

# 📌 Información General

**Asignatura:** Programación / Desarrollo de Interfaces Gráficas  
**Unidad:** Unidad 1  
**Alumno:** Luis Angel  
**Lenguaje de programación:** Python  
**Framework utilizado:** Flet  
**Tipo de aplicación:** Formulario Web Interactivo  
**Entorno de ejecución:** Navegador Web  

---

# 📖 Marco Teórico

La validación de datos constituye uno de los pilares fundamentales en el desarrollo de software moderno. Un sistema que no valida correctamente la información de entrada puede generar inconsistencias, errores lógicos y vulnerabilidades.

En el desarrollo de interfaces gráficas, es indispensable garantizar que:

- Los campos obligatorios sean completados.
- Los formatos de datos sean correctos.
- Los valores ingresados cumplan restricciones específicas.
- El usuario reciba retroalimentación inmediata ante errores.

El framework **Flet** permite construir interfaces interactivas utilizando Python, facilitando la creación de aplicaciones web sin necesidad de emplear tecnologías tradicionales como HTML, CSS o JavaScript de forma directa.

Este proyecto representa una aplicación práctica de dichos principios mediante la creación de un formulario académico con múltiples validaciones.

---

# 🎯 Objetivo General

Desarrollar un formulario web interactivo que capture información académica y aplique validaciones estrictas antes de permitir el procesamiento de los datos.

---

# 🎯 Objetivos Específicos

- Diseñar una interfaz gráfica clara, organizada y centrada.
- Implementar validaciones para evitar campos vacíos.
- Restringir el campo “Número de control” a valores numéricos.
- Validar el formato del correo electrónico mediante expresiones regulares.
- Implementar controles gráficos avanzados como Dropdown y RadioGroup.
- Mostrar dinámicamente la información ingresada después de ser validada.

---

# 🧩 Descripción General del Sistema

El sistema desarrollado consiste en un formulario académico que permite capturar los siguientes datos:

1. Nombre completo del alumno  
2. Número de control  
3. Correo electrónico  
4. Carrera  
5. Semestre (selección desde menú desplegable)  
6. Género (selección mediante botones de opción)

La interfaz se encuentra organizada dentro de un contenedor principal con diseño centrado, fondo claro y estructura vertical mediante columnas.

El sistema interactúa con el usuario en tiempo real, evaluando los datos ingresados antes de permitir su envío.

---

# 🛠️ Componentes y Controles Utilizados

El formulario hace uso de los siguientes componentes del framework Flet:

- **TextField** → Captura de texto.
- **Dropdown** → Selección estructurada de opciones.
- **RadioGroup** → Selección exclusiva entre múltiples opciones.
- **ElevatedButton** → Activación del evento de validación.
- **Text** → Mensajes dinámicos y resultados.
- **Container, Column y Row** → Organización visual y estructura.

Cada componente cumple una función específica dentro del flujo de interacción del usuario.

---

# ✅ Validaciones Implementadas

## 1️⃣ Campos Obligatorios

Todos los campos del formulario deben ser completados antes de enviar la información.

Si un campo se encuentra vacío:

- Se resalta visualmente.
- Se impide el envío del formulario.
- Se muestra un mensaje de advertencia.

---

## 2️⃣ Validación de Número de Control (Solo Números)

Se implementó una función que filtra cualquier carácter que no sea numérico:

```python
def solo_numeros(e):
    control.value = ''.join(filter(str.isdigit, control.value))
    page.update()
```

Esta función elimina automáticamente letras y símbolos, permitiendo únicamente números.

---

## 3️⃣ Validación de Correo Electrónico

Se utiliza una expresión regular para validar el formato del correo electrónico:

```python
patron = r"^[a-zA-Z0-9._%+-]+@gmail\.com$"
```

La validación garantiza:

- Formato estructural correcto.
- Dominio obligatorio @gmail.com.
- Ausencia de caracteres inválidos.

---

## 4️⃣ Validación de Selección de Semestre

El usuario debe seleccionar un semestre desde el menú desplegable antes de continuar.

---

## 5️⃣ Validación de Selección de Género

El sistema exige que se seleccione una opción dentro del grupo de género antes de enviar la información.

---

# 🔄 Flujo de Funcionamiento

Cuando el usuario presiona el botón **Enviar**, el sistema:

1. Reinicia estilos de error.
2. Evalúa cada campo individualmente.
3. Verifica campos obligatorios.
4. Valida formato de correo.
5. Confirma selección de opciones.
6. Si todo es correcto, muestra los datos ingresados.

Este comportamiento está basado en programación orientada a eventos.

---

# 🖼️ Evidencia Visual del Sistema
---

## 📸 Captura 1 – Vista General del Formulario

<img width="1920" height="1128" alt="image" src="https://github.com/user-attachments/assets/0359dde4-e753-4f41-abdd-93789b6bf17e" />


---

## 📸 Captura 2 – Ejemplo de Validación de Error

<img width="1920" height="1128" alt="image" src="https://github.com/user-attachments/assets/06db6801-c36e-4f54-9276-4bad53ae8ba7" />


---

## 📸 Captura 3 – Datos Enviados Correctamente

<img width="1920" height="1128" alt="image" src="https://github.com/user-attachments/assets/75eabcb0-14f9-4c41-8846-f98a526e651a" />

---

# 🎓 Conclusión

El presente proyecto permitió integrar conocimientos fundamentales de programación y diseño de interfaces gráficas mediante la construcción de un sistema funcional con validaciones estructuradas.

Se logró desarrollar un formulario interactivo capaz de:

- Restringir entradas inválidas.
- Validar información en tiempo real.
- Proporcionar retroalimentación visual al usuario.
- Organizar componentes de forma estructurada y profesional.

Este trabajo representa una base sólida para futuros desarrollos de aplicaciones web más complejas, fortaleciendo las competencias en Python y en el uso del framework Flet.
