# CleanYourTV — Guía de instalación

## Requisitos

- Android TV o Google TV.
- Python 3, Git, Android SDK y Java para compilar.
- Ordenador y televisor conectados a la misma red.
- Depuración ADB por red habilitada.

## Descargar el repositorio

`git clone https://github.com/Gathin23/cleanyourtv.git`

## Preparar el entorno

`python3 -m venv tools/venv`

`tools/venv/bin/pip install -r tools/requirements.txt`

## Conectar el televisor

Define la IP real del televisor:

`export TV_HOST=192.168.1.100`

Comprueba la conexión:

`TV_HOST=$TV_HOST tools/venv/bin/python -I tools/tv.py --probe`

## Instalar CleanYourTV

`TV_HOST=$TV_HOST launcher/build-and-install.sh`

## Instalar un tema

Consulta los temas disponibles en `themes/README.md`. Ejemplo:

`TV_HOST=$TV_HOST tools/theme.sh themes/neon-aurora`

## Restauración y ayuda

- [Restauración](restore.md)
- [Preguntas frecuentes](faq.md)
- [Solución de problemas](TROUBLESHOOTING.md)
- [Recomendaciones de seguridad](DOS-AND-DONTS.md)

## Seguridad

- No desinstales aplicaciones del fabricante sin conocer su función.
- No desactives componentes del sistema.
- Revisa la restauración antes de cambiar el launcher predeterminado.
- Deshabilita ADB cuando no lo necesites.
- Haz una copia de seguridad antes de realizar cambios importantes.

Consulta también el [README principal](../README.md).
