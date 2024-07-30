    <h1>Tetris en Python</h1>

    <p>Este proyecto es una implementación simplificada del juego clásico Tetris en Python. Utiliza la biblioteca <code>keyboard</code> para la entrada del teclado y <code>threading</code> para la caída automática de las piezas.</p>

    <h2>Requisitos</h2>
    <p>Para ejecutar el juego, necesitas tener instaladas las siguientes bibliotecas de Python:</p>
    <ul>
        <li><code>keyboard</code></li>
    </ul>
    <p>Puedes instalarla usando pip:</p>
    <pre><code>pip install keyboard</code></pre>

    <h2>Descripción</h2>
    <p>El juego Tetris en este proyecto se ejecuta en la consola. Las piezas caen automáticamente y puedes moverlas usando las teclas del teclado. El objetivo es completar filas horizontales en el tablero para que desaparezcan y ganes puntos.</p>

    <h2>Cómo Jugar</h2>
    <ul>
        <li><strong>Mover la pieza hacia abajo:</strong> Usa la tecla de flecha hacia abajo (<code>↓</code>), <code>s</code> o <code>down</code>.</li>
        <li><strong>Mover la pieza a la derecha:</strong> Usa la tecla de flecha hacia la derecha (<code>→</code>), <code>d</code> o <code>right</code>.</li>
        <li><strong>Mover la pieza a la izquierda:</strong> Usa la tecla de flecha hacia la izquierda (<code>←</code>), <code>a</code> o <code>left</code>.</li>
        <li><strong>Rotar la pieza:</strong> Usa la barra espaciadora (<code>space</code>).</li>
        <li><strong>Salir del juego:</strong> Presiona la tecla <code>ESC</code>.</li>
    </ul>

    <h2>Cómo Ejecutar el Juego</h2>
    <ol>
        <li>Guarda el código en un archivo llamado <code>tetris.py</code> (o cualquier otro nombre que prefieras).</li>
        <li>Ejecuta el archivo con Python:</li>
    </ol>
    <pre><code>python tetris.py</code></pre>

    <h2>Estructura del Código</h2>
    <h3>Clases Principales</h3>
    <ul>
        <li><strong><code>Board</code></strong>: Representa el tablero de juego. Maneja la impresión del tablero, el movimiento de las piezas y la eliminación de filas completas.</li>
        <li><strong><code>Piece</code></strong>: Representa una pieza del Tetris. Tiene un color, una forma y un estado de rotación.</li>
        <li><strong>Bloques (<code>_JBlock</code>, <code>_IBlock</code>, <code>_LBlock</code>, <code>_SquareBlock</code>, <code>_TBlock</code>, <code>_ZBlock</code>, <code>_SBlock</code>)</strong>: Definen las diferentes formas de las piezas del Tetris.</li>
    </ul>

    <h3>Métodos Clave</h3>
    <ul>
        <li><strong><code>print_board</code></strong>: Limpia la pantalla y muestra el tablero con la pieza actual.</li>
        <li><strong><code>update_board</code></strong>: Actualiza el tablero con la pieza actual y genera una nueva pieza.</li>
        <li><strong><code>move_piece</code></strong>: Mueve la pieza actual en el tablero según la entrada del usuario.</li>
        <li><strong><code>_rotate_shape</code></strong>: Calcula las nuevas posiciones de una pieza después de rotarla utilizando álgebra lineal.</li>
        <li><strong><code>_is_valid_move</code></strong>: Verifica si un movimiento es válido para la pieza actual.</li>
        <li><strong><code>_full_row_control</code></strong>: Elimina las filas completas y agrega nuevas filas vacías en la parte superior.</li>
    </ul>

    <h2>Ejemplos de Uso</h2>
    <p>Para comenzar a jugar, simplemente ejecuta el script y usa las teclas indicadas para mover y rotar las piezas. El juego continuará hasta que no haya espacio para nuevas piezas en la parte superior del tablero.</p>

    <h2>Contribuciones</h2>
    <p>Si tienes ideas para mejorar el juego o encuentras errores, siéntete libre de contribuir al proyecto. Puedes hacer un fork del repositorio y enviar una solicitud de extracción con tus cambios.</p>

    <h2>Licencia</h2>
    <p>Este proyecto está bajo la Licencia MIT. Consulta el archivo <code>LICENSE</code> para obtener más detalles.</p>
</body>
</html>
