from flask import Flask, url_for

app = Flask(__name__)


@app.route('/')
@app.route('/serv')
def serv():
    return "Миссия Колонизация Марса"


@app.route('/index')
def index():
    return "И на Марсе будут яблони цвести!"


@app.route('/promotion')
def promotion():
    return """  <p>Человечество вырастает из детства.</p>
                <p>Человечеству мала одна планета.</p>
                <p>Мы сделаем обитаемыми безжизненные пока планеты.</p>
                <p>И начнем с Марса!</p>
                <p>Присоединяйся!</p>"""


@app.route('/image_mars')
def image_mars():
    return """<html>
    <head>
        <title>
            Привет, Марс!
        </title>
    </head>
    <body>
        <h1>Жди нас, Марс!</h1>
        <img src="{}" alt="здесь должна была быть картинка, но не нашлась">
    </body>
    </html>""".format(url_for('static', filename='img/mars.jpg'))


if __name__ == '__main__':
    app.run(port=8080, host='127.0.0.1')
