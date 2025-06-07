# 📋 Automação de Consulta de Débitos no Sistema NewCon

Este projeto automatiza o preenchimento de dados no sistema **NewCon** para facilitar a consulta e verificação de débitos relacionados a grupos e cotas, utilizando informações provenientes de uma planilha Excel.

A automação simula ações humanas com o uso do **PyAutoGUI** para navegação, preenchimento e interação com o sistema, gerando mais agilidade e precisão no processo.

---

## 🚀 Funcionalidades

- Abertura automatizada do navegador e acesso ao sistema NewCon
- Navegação até o módulo "Planilha de Débitos"
- Leitura de uma planilha `.xlsx` contendo os dados de grupo, cota e versão
- Preenchimento automático dos campos no sistema
- Interação com menus e opções por meio de atalhos visuais com reconhecimento de imagem

---

## 📂 Estrutura Esperada da Planilha

A planilha `.xlsx` deve conter os seguintes campos na aba **Teste**:

| Grupo | Cota | Versão |
|--------|------|--------|
| 123    | 456  | A      |

---

## 🧰 Tecnologias Utilizadas

- [Python 3.x](https://www.python.org/)
- [PyAutoGUI](https://pyautogui.readthedocs.io/en/latest/) – Automação de teclado, mouse e reconhecimento de imagens
- [OpenPyXL](https://openpyxl.readthedocs.io/en/stable/) – Leitura da planilha Excel
- [Pillow (PIL)](https://pillow.readthedocs.io/en/stable/) – Manipulação de imagens para detecção visual (requerido pelo PyAutoGUI)

---

## ▶️ Como Usar

1. Instale os pacotes necessários:

```bash
pip install pyautogui openpyxl pillow
```

2. Ajuste a resolução e os atalhos visuais do sistema para que correspondam às imagens utilizadas no script (`atalhos_newcon.png`, `planilha_de_debitos.png`, etc.)

3. Coloque a planilha `cotas_inicio_proc.xlsx` no mesmo diretório do script.

4. Execute o script:

```bash
python planilha_de_debitos_v3.py
```

> ⚠️ Durante a execução, **não mova o mouse ou interfira nas ações do sistema**, pois isso pode interromper ou desconfigurar o processo.

---

## ✅ Requisitos

- Sistema NewCon deve estar acessível via navegador (Google Chrome)
- Resolução de tela e escala compatíveis com os prints utilizados para reconhecimento visual
- Contas e permissões necessárias para acessar os dados de débitos

---

## 🧩 Sugestões

- Utilizar um monitor ou máquina dedicada para execução da automação
- Incluir tratamento de erros ou geração de relatórios para logs e cotas não processadas
- Agendar execuções com ferramentas como `cron` (Linux) ou `Agendador de Tarefas` (Windows)

---

👨‍💻 Autor Rodrigo de Lima Aleixo 
💼 [LinkedIn](https://www.linkedin.com/in/rodrigo-de-lima-aleixo-850b1720b/)
✉️ E-mail: *rodriigoaleixo@gmail.com*

Feito para reduzir o retrabalho e aumentar a produtividade com automação! 🤖✨
