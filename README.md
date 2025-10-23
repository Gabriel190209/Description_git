# Atividade de Colaboração em Repositório Git/GitHub

Este documento detalha os passos realizados para clonar um repositório, criar uma nova *branch* para documentação, fazer as alterações necessárias, subir as mudanças para o GitHub e criar um *Pull Request* (PR), simulando um fluxo de colaboração.

---

## 🧑‍🤝‍🧑1. Clonagem do Repositório (Fork/Clone)

Inicialmente, o repositório foi clonado do GitHub para a máquina local usando o comando `git clone`.

* **Comando:** `git clone https://github.com/Gabriel190209/git-local.git`
* **Ação:** Baixa todos os arquivos e o histórico do repositório remoto para o diretório local `git-local`.

## 🚢2. Navegação e Criação de Branch

Após a clonagem, naveguei para o diretório do projeto e criei uma nova *branch* específica para a documentação e colaboração.

* **Comando para Navegar:** `cd git-local`
* **Comando para Criar e Mudar de Branch:** `git checkout -b documentacao-colaboracao`
* **Resultado:** A *branch* `documentacao-colaboracao` foi criada e o ambiente de trabalho foi imediatamente trocado para ela.

<div align="center">
  <img width="518" height="252" alt="1parte" src="https://github.com/user-attachments/assets/d8d78808-db69-46b7-8b42-109d47aa44ba" />
</div>

---

## 🔍3. Verificação do Status e Branches

Após o *push*, o *status* da *branch* local foi verificado, e uma lista das *branches* local e remota foi exibida.

* **Comando para Listar Branches:** `git branch -a`
    * Mostra: `main` (local), `documentacao-colaboracao` (local e remota), `origin/main` (remota).
* **Comando para Status:** `git status`
    * Confirma que a *branch* local está sincronizada com a remota (`up to date with 'origin/documentacao-colaboracao'`) e que não há alterações pendentes.

<div align="center">
  <img width="568" height="441" alt="parte2" src="https://github.com/user-attachments/assets/465d4d38-e831-41f2-a33e-9908dbf6e841" />
</div>

---

## ✅4. Realização e Commit das Alterações (Simulado)

*Neste ponto, as alterações nos arquivos (como a documentação sobre integração e colaboração) foram realizadas, embora não mostradas diretamente.*

Em seguida, os arquivos alterados foram adicionados ao *staging area* e um *commit* foi realizado com uma mensagem descritiva (seguindo, neste caso, a convenção *feat* - *feature*).

* **Comando para Adicionar:** `git add .` (Adiciona todos os arquivos modificados/novos)
* **Comando para Commit:** `git commit -m "feat: Adiciona documentacao sobre integracao e colaboracao"`

*Observação na Imagem:* A imagem `parte3.png` mostra um *commit* sendo executado, mas em seguida, mostra que a *branch* local já estava "up to date" e o *working tree clean*, o que pode indicar que um *commit* anterior não foi totalmente gravado ou a imagem foi tirada após uma tentativa de *commit* sem alterações pendentes. O comando de *commit* em si foi executado.

## 📨5. Envio da Branch para o Repositório Remoto (Push)

O código da nova *branch* local foi enviado para o GitHub.

* **Comando:** `git push -u origin documentacao-colaboracao`
    * O `-u` (ou `--set-upstream`) garante que o Git saiba para qual *branch* remota enviar futuros `git push` ou `git pull`.
* **Resultado:** A *branch* `documentacao-colaboracao` foi criada no repositório remoto. O terminal inclusive sugere o link direto para criar o Pull Request.

<div align="center">
  <img width="536" height="184" alt="parte3" src="https://github.com/user-attachments/assets/2d2b0d5f-a491-45ec-b8c6-6c60051fe242" />
</div>

---

## ⚙️6. Configuração de Colaboradores (Contexto de Colaboração)

Para permitir a colaboração e a revisão do código, convites foram enviados a outros usuários para serem colaboradores do repositório.

* **Ação:** No painel de `Settings` (Configurações) > `Collaborators` (Colaboradores) do GitHub, foram adicionados usuários como `Pedro Ferracioli`, `leo`, e `TiagoPadovaniCardoso`.
* **Status:** Os convites estavam em estado "Pending Invite" (Convite Pendente).

<div align="center">
  <img width="1902" height="937" alt="InviteGente" src="https://github.com/user-attachments/assets/fb21bd5b-c48f-4eef-8452-4d3f615dc2d5" />
</div>

---

## 💾7. Criação do Pull Request (PR)

No GitHub, a interface de comparação de mudanças foi acessada para iniciar a criação de um *Pull Request*.

* **Base:** `leonardo27032009/inicial-git` (base branch `main`) - *Observação: Base em um fork, comum em fluxos de contribuição.*
* **Head (Mudança):** `Gabriel190209/inicial-git-leo` (head branch `main`) - *Observação: O PR está comparando branches main entre repositórios que parecem ser forks.*

* **Ação (Implícita):** Embora a imagem mostre uma comparação entre *forks* (o que é um fluxo comum de contribuição externa), a intenção final é criar o **Pull Request** (`Create pull request`) para propor a integração da alteração (`Update README.md` - 1 commit, 1 file changed) na *branch* principal.
* **Status:** `Able to merge. These branches can be automatically merged.` (Pronto para a fusão automática).

<div align="center">
  <img width="1254" height="462" alt="CreatePull" src="https://github.com/user-attachments/assets/d5670d5e-9c1d-499f-8a2f-d66ee98b57dd" />
</div>

---

## 🚀 Conclusão

Os passos acima demonstram o ciclo completo de um fluxo de trabalho baseado em *branching* e *Pull Request* para a inclusão de uma nova *feature* ou documentação em um projeto, incluindo a configuração de colaboradores para revisão e aprovação.

<div align="center">
  <img width="944" height="483" alt="Captura de tela 2025-10-23 164834" src="https://github.com/user-attachments/assets/ef790479-191b-41bd-a823-434305fae1d4" />
</div>
