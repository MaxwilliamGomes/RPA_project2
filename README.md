# 📱 WhatsApp Contact Extractor

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Selenium](https://img.shields.io/badge/Selenium-4.0+-green.svg)](https://www.selenium.dev/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3+-orange.svg)](https://pandas.pydata.org/)

## 📋 Descrição do Projeto

Este projeto de RPA (Robotic Process Automation) automatiza a extração de contatos de grupos do WhatsApp Web, processa os dados com Python e gera um arquivo CSV organizado. Uma solução eficiente para quem precisa exportar contatos de grupos do WhatsApp para uso em outras plataformas ou análises.

## 🔄 Fluxo de Trabalho

```mermaid
graph LR
    A[WhatsApp Web] -->|Extração de contatos via Selenium| B[Python - Processamento de dados]
    B -->|Limpeza e formatação| C[Arquivo CSV]
    C -->|Disponível para uso em outras ferramentas| D[Análises/Integrações]
```

## ✨ Funcionalidades

- **Acesso Automatizado ao WhatsApp Web**: Utiliza Selenium para acessar a interface web
- **Extração de Contatos**: Captura números de telefone de participantes do grupo
- **Processamento de Dados**: Limpa e formata os números para padronização
- **Geração de Links Diretos**: Cria URLs para iniciar conversas via WhatsApp Web
- **Exportação para CSV**: Salva os contatos em formato organizado e pronto para uso

## 🛠️ Pré-requisitos

- Python 3.9+
- Chrome ou Chromium instalado
- Bibliotecas Python:
  - selenium
  - pandas
  - webdriver-manager
  - re (built-in)
  - warnings (built-in)

## 📦 Instalação

```bash
# Clonar o repositório
git clone https://github.com/MaxwilliamGomes/RPA_project2.git
cd RPA_project2

# Instalar dependências
pip install -r requirements.txt
```

## 🚀 Como Usar

1. **Execute o script principal**:
   ```bash
   jupyter notebook src/Main.ipynb
   ```

2. **Autenticação no WhatsApp Web**:
   - Quando o navegador abrir, escaneie o código QR com seu celular
   - Aguarde a autenticação completa

3. **Navegue até o grupo desejado**:
   - Abra o grupo do WhatsApp cujos contatos deseja extrair
   - Clique no título do grupo para ver os participantes

4. **Execute as células do notebook sequencialmente**:
   - O script irá extrair os números de telefone
   - Processar e limpar os dados
   - Gerar um arquivo CSV com os contatos

5. **O arquivo CSV será salvo** como `contatos_whatsapp.csv` no diretório de trabalho


```

## 📊 Estrutura do Arquivo CSV Gerado

| Whatsapp         | Link                                            | Grupo         |
|------------------|-------------------------------------------------|---------------|
| numero           | link do whatsapp do contato                     | Nome do grupo |


## ⚠️ Considerações Importantes

- **Privacidade**: Utilize este script apenas para grupos onde você tem permissão para acessar os contatos
- **Termos de Serviço**: Observe os Termos de Serviço do WhatsApp ao utilizar esta automação
- **Limitações**: O WhatsApp pode modificar sua interface, o que pode exigir atualizações no código
- **Uso Responsável**: Não utilize os contatos extraídos para spam ou comunicações não autorizadas

## 🔄 Possíveis Melhorias

- Implementar extração de múltiplos grupos
- Adicionar suporte a extração de outros dados como foto de perfil e status
- Criar interface gráfica para facilitar o uso
- Adicionar opção para exportar em outros formatos (Excel, JSON)





