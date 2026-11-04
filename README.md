# 🛡️ Laboratório de Análise de Ameaças: Simulação de Ransomware e Keylogger em Python

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Security](https://img.shields.io/badge/Domain-Cybersecurity_Defensive-red)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

## 📌 Descrição do Projeto
Este projeto foi desenvolvido para fins estritamente educacionais e de pesquisa no âmbito da segurança da informação. O objetivo é demonstrar de forma prática o funcionamento lógico de duas das ameaças cibernéticas mais comuns — **Ransomware** e **Keylogger** —, utilizando a linguagem **Python** em um ambiente isolado, visando compreender os vetores de ataque para implementar defesas eficazes.

---

## ⚙️ Cenários Implementados

### 1. Ransomware Simulado
* **Funcionamento:** Utiliza a biblioteca `cryptography` (Fernet) para gerar uma chave simétrica, criptografar arquivos de texto de teste (`teste_dados.txt`) e gerar um arquivo de aviso de resgate (`LEIA_ISSO.txt`).
* **Mitigação:** Demonstra a importância de manter rotinas de **backup offline (regra 3-2-1)** e políticas rígidas de controle de acesso a arquivos sensíveis.

### 2. Keylogger Simulado
* **Funcionamento:** Utiliza a biblioteca `pynput` para escutar e registrar eventos de digitação do teclado em um arquivo de texto local (`log_teclas.txt`).
* **Mitigação:** Evidencia a necessidade de uso de **soluções EDR/Antivírus modernos** capazes de detectar requisições de *hooks* globais no sistema operacional e o uso de teclados virtuais para inserção de senhas críticas.

---

## 🚀 Como Executar o Laboratório (Ambiente Seguro)

1. Clone o repositório em uma máquina virtual isolada:
   ```bash
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
   cd seu-repositorio
