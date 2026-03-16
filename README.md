# 🚀 Lead Scraper | High Performance Dashboard

O **Lead Scraper** é uma ferramenta de alta performance executada inteiramente no navegador. Ela permite a importação, armazenamento local e visualização de milhares de leads (empresas/contatos) a partir de arquivos CSV, utilizando a tecnologia **IndexedDB** para garantir que os dados permaneçam salvos mesmo após fechar o navegador.

![Versão](https://img.shields.io/badge/Vers%C3%A3o-1.0-blue)
![Tech](https://img.shields.io/badge/Tech-HTML5%20%7C%20JS%20%7C%20Bootstrap-green)
![Storage](https://img.shields.io/badge/Storage-IndexedDB-orange)

---

## ✨ Funcionalidades

* **Importação Ultra-Rápida:** Processa arquivos CSV pesados em segundos utilizando streaming de dados (PapaParse).
* **Busca Global Instantânea:** Filtre por CNPJ, Razão Social, Cidade ou código CNAE em tempo real.
* **Armazenamento Local:** Os dados ficam salvos no seu navegador (não precisa de banco de dados externo ou servidor).
* **Integração com WhatsApp:** Clique no ícone para abrir o chat diretamente com o número do lead.
* **Paginação Inteligente:** Renderiza apenas 50 registros por vez para manter a fluidez, mesmo com 100.000+ linhas.
* **Design Responsivo:** Interface moderna construída com Bootstrap 5, otimizada para Desktop e Mobile.

---

## 🛠️ Como Usar

1.  **Abrir a Ferramenta:** Basta abrir o arquivo `.html` em qualquer navegador moderno (Chrome, Edge ou Firefox).
2.  **Importar Dados:** Clique no botão **"Importar CSV"** no topo da página e selecione seu arquivo.
3.  **Aguardar Processamento:** Uma barra de carregamento indicará o progresso. Ao terminar, seus leads aparecerão na tabela.
4.  **Navegar e Buscar:** Utilize a barra de busca superior para filtragem instantânea.
5.  **Limpar Banco:** Para subir uma nova lista do zero, utilize o botão **"Limpar Banco"**.

---

## 📋 Estrutura do CSV Suportada

Para que os dados apareçam corretamente, seu arquivo CSV deve conter os seguintes cabeçalhos (nomes das colunas):

| Coluna | Descrição |
| :--- | :--- |
| **CNPJ** | Identificador único (obrigatório para salvar). |
| **RAZAO SOCIAL** | Nome jurídico da empresa. |
| **FANTASIA** | Nome comercial/nome de fachada. |
| **TELEFONE** | Telefone com DDD (ex: 88999998888). |
| **DESC CNAE** | Descrição da atividade econômica. |
| **CIDADE** | Cidade de origem. |
| **UF** | Estado (ex: CE, SP, RJ). |

> **Dica:** O sistema detecta automaticamente se o separador do seu CSV é vírgula (,) ou ponto e vírgula (;).

---

## 🚀 Tecnologias Utilizadas

* **Bootstrap 5:** Layout e componentes visuais.
* **Font Awesome 4.7:** Ícones de interface.
* **PapaParse:** Biblioteca de alta performance para parsing de CSV.
* **IndexedDB:** Banco de dados NoSQL nativo do navegador para persistência de dados em larga escala.

---

## ⚠️ Observações Importantes

* **Privacidade:** Seus dados **não** são enviados para nenhum servidor. Tudo é processado localmente na sua máquina (Client-side).
* **Limpeza de Cache:** Se você limpar os "Dados de Sites" ou o cache do navegador de forma profunda, os leads salvos no IndexedDB serão apagados.
* **Performance:** A ferramenta foi otimizada para lidar com grandes volumes (100k+ registros) sem travar a interface.

---

**Desenvolvido para alta performance em prospecção B2B.**
