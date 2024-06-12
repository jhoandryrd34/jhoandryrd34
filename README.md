graph TD;
    A[Abrir página de notas] -->|GET| B(HTML document)
    B -->|GET| C{main.css}
    C -->|GET| D{main.js}
    D -->|Ejecución| E{Fetch JSON data}
    E -->|GET| F(JSON data)
    F -->|Renderizar| G[Notas]
    H[Usuario crea nueva nota] -->|POST| I(Servidor)
    I -->|Actualización| F
