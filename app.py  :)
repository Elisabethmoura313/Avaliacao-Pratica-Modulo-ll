from flask import Flask, request, render_template, jsonify

app = Flask(__name__) # vai definir a rota ✨

@app.route("/soma", methods=['GET'])
def get_soma():
    valor1 = float(request.args.get("valor1")) 
    valor2 = float(request.args.get("valor2")) 
    somar = valor1 + valor2
    return jsonify({"resultado": somar})

@app.route("/subtracao", methods=['GET'])
def get_subtracao():
    valor1 = float(request.args.get("valor1")) 
    valor2 = float(request.args.get("valor2")) 
    get_subtracao = valor1 - valor2
    return jsonify({"resultado": get_subtracao})

@app.route("/multiplicar", methods=['GET'])
def get_multiplicar():
    valor1 = float(request.args.get("valor1")) 
    valor2 = float(request.args.get("valor2")) 
    get_multiplicar = valor1 * valor2
    return jsonify({"resultado": get_multiplicar})

@app.route("/dividir", methods=['GET'])
def get_dividir():
    valor1 = float(request.args.get("valor1")) 
    valor2 = float(request.args.get("valor2")) 
    if valor2 == 0:
        return jsonify({"erro": "Divisão por zero não é permitida"})
    get_dividir = valor1 / valor2
    return jsonify({"resultado": get_dividir})

if __name__ == "__main__":
    app.run(debug=True)
