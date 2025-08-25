import flask
from flask import Flask


app = Flask(__name__)
@app.route('/')
def main():
    return 'HOla, todos!'

@app.route('/saluda/clase')
def saluda_clase():
    return "<marquee><h1>Hola, clase!</h1></marquee>"
if __name__ == '__main__':
    app.run()
