# Conversor de Moeda

<img src="https://user-images.githubusercontent.com/29135156/81971272-35c84700-95f7-11ea-845d-c8732181bb00.gif" width="100%" heigth="auto">

Este projeto nós desenvolvemos um app que realiza conversções entre real, dolar e euro.
A finalidade deste projeto é apresentar diversos recursos do Flutter, entre eles a reutilização dos Widgets, através de uma função genérica podemos passar parâmetros e utilizar a função para TextFields semelhantes ou outros controles.

<pre>
    <code>
        Widget buildTextField(String label, String prefix, TextEditingController controller, Function funcao) {
            return TextField(
                decoration: InputDecoration(
                    labelText: label,
                    labelStyle: TextStyle(color: Colors.amber),
                    border: OutlineInputBorder(),
                    prefixText: prefix),
                style: TextStyle(color: Colors.amber, fontSize: 25.0),
                controller: controller,
                onChanged: funcao,
                keyboardType: TextInputType.numberWithOptions(decimal: true),
            );
        }
    </code>
</pre>

<pre>
    <code>
        buildTextField("Reais", "R\$", realController, _realChanged),
    </code>
</pre>

## Introdução

Alguns recursos para você começar se este for seu primeiro projeto Flutter:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

Para obter ajuda sobre como iniciar o Flutter, consulte nosso
[online documentation](https://flutter.dev/docs), que oferece tutoriais,
amostras, orientações sobre desenvolvimento móvel e uma referência completa da API.
