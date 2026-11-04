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
* Arquivos e código utilizado localizado
malware/dec_ransomware.py 
e malware/enc_ransomware.py

### 2. Keylogger Simulado
* **Funcionamento:** Utiliza a biblioteca `pynput` para escutar e registrar eventos de digitação do teclado em um arquivo de texto local (`log_teclas.txt`).
```bash
pip install pynput --break-system-packages
```
```bash
python Keylogger/Kaylogger.py  
```
Códigos utilizado e arquivos estão localizados nos caminhos 
malware/keylogger.py
malware/keylogger_email.pyw

* **Mitigação:** Evidencia a necessidade de uso de **soluções EDR/Antivírus modernos** capazes de detectar requisições de *hooks* globais no sistema operacional e o uso de teclados virtuais para inserção de senhas críticas.

---

## 🚀 Como Executar o Laboratório (Ambiente Seguro)
Use uma máquina virtual ou um ambiente local protegido.



## 🛡️ Medidas de Defesa e Conscientização

Para proteger ambientes corporativos e domésticos contra essas ameaças, recomenda-se:

Conscientização do Usuário: Treinamentos periódicos contra phishing e engenharia social (vetor primário de infecção).

Princípio do Menor Privilégio: Evitar o uso de contas com privilégios de Administrador/Root para tarefas cotidianas.

Segmentação de Rede e Firewall: Bloquear comunicações de C2 (Command and Control) não autorizadas.

Soluções Antivírus Atualizadas: Utilizar varreduras comportamentais em tempo real.

Desenvolvido por LIBERATO durante os estudos práticos de Cibersegurança na DIO.
