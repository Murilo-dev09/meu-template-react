
Abra o terminal e vá para a pasta onde quer salvar o projeto.
Exemplo (Windows):

cd Desktop\Docs


(No macOS / Linux: cd ~/Desktop/Docs)

Clone o repositório:

git clone https://github.com/murilo-dev09/meu-template-react.git


Entre na pasta do projeto:

cd meu-template-react


Abra no VS Code (opcional):

code .


Instale as dependências:

npm install


Rode o projeto:

npm run dev


Depois abra o link que aparecer (ex.: http://localhost:5173).

✅ Pontos importantes / recomendações

Certifique-se de ter Git e Node.js (com npm) instalados.

Verificar Git: git --version

Verificar Node: node --version e npm --version

Se não tiver Git no computador, pode baixar o ZIP no GitHub (botão Code → Download ZIP), extrair e seguir os passos a partir do passo 3.

Se aparecer erro no Windows sobre execução de scripts (npm.ps1), rode no PowerShell como administrador:

Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned


e depois tente npm install de novo.

🛠️ Troubleshooting rápido

Tela branca / nada aparece? Confere se index.html tem <div id="root"></div> e se main.jsx está referenciando App.jsx corretamente.

Imagem não aparece: verifique se imagens usadas com src="/imagens/..." estão na pasta public/imagens/. Se estiverem em src/assets, importe via import banner from '../assets/banner.png'.

Erro de dependência: delete node_modules e package-lock.json e rode npm install de novo.
