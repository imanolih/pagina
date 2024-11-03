import streamlit as st

# Título de la aplicación
st.title("Mi primera aplicación de Streamlit")

# Texto de bienvenida
st.header("¡Hola, Streamlit!")
st.write("Esta es una aplicación simple")

# Agrega una imagen (opcional)
st.image("C:\Users\Ignacio Manoli\OneDrive\Desktop", caption="UNIVERSIDAD SAN SEBASTIAN", use_column_width=True)

# Botón de clic
if st.button("Haz clic"):
    st.write("¡Has hecho clic en el botón!")

# Entrada de texto
user_input = st.text_input("Escribe algo:")
st.write("Escribiste:", user_input)

# Barra lateral
st.sidebar.title("Mi primera barra lateral de Streamlit")
st.sidebar.write("Esto es una barra lateral")

# Agrega una imagen a la barra lateral
st.sidebar.image("ruta/de/tu/logo.png", use_column_width=True)

# Botón y entrada de texto en la barra lateral
if st.sidebar.button("Haz clic pero en la barra lateral"):
    st.sidebar.write("¡Haz hecho clic en la barra lateral!")

barra_input = st.sidebar.text_input("Escríbete en la barra:")
st.sidebar.write("Escribiste en la barra:", barra_input)
