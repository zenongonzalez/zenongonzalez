- 👋 Hi, I’m @zenongonzalez
- 👀 I’m interested in PROGRAMACION Y DESARROLLO WEB...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
#!/usr/bin/env python
# -*- coding: UTF-8 -*-
import web
from web import form

urls = ('/', 'ingreso')

app = web.application(urls, globals())

# Creamos nustro formulario:
login = form.Form(form.Textbox('usuario'),form.Password('clave'),form.Button('Iniciar'))

class ingreso:
    def GET(self):
        f = login()
        return f.render()

def main():
    app.run()
    return 0

if __name__ == "__main__": 
    main()
<!---
zenongonzalez/zenongonzalez is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
