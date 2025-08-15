# 💻 Workstation Tools

Este repositório contém *playbooks* e scripts para automatizar e agilizar a configuração inicial da minha máquina de trabalho, instalando ferramentas essenciais para desenvolvimento e operações.

> **Aviso:**  
> O arquivo `ubuntu.yml` é voltado para **Ubuntu** (versão 18.04 ou superior). 
> O arquivo `zorin-os.yml` é voltado para **Zorin OS**.  
> Para **openSUSE**, utilize o `opensuse.yml`.  
> Outras distribuições podem exigir adaptações.

---

## 📦 Preparar Estação de Trabalho

### 🔹 Ubuntu (18.04+)

1. **Instale o Ansible e dependências**  
```bash
sudo apt update && sudo apt install ansible unzip git -y
```

2. **Clone este repositório**  
```bash
git clone https://github.com/silvemerson/tools.git
cd tools
```

3. **Aplique a configuração**  
```bash
ansible-playbook ubuntu.yml --ask-become-pass
```
> Quando solicitado, digite sua senha para conceder permissões administrativas.

---

### 🔹 openSUSE (Leap ou Tumbleweed)

1. **Instale o Ansible e dependências**  
```bash
sudo zypper refresh
sudo zypper install ansible unzip git -y
```

2. **Clone este repositório**  
```bash
git clone https://github.com/silvemerson/tools.git
cd tools
```

3. **Aplique a configuração**  
```bash
ansible-playbook opensuse.yml --ask-become-pass
```
> Quando solicitado, digite sua senha para conceder permissões administrativas.

---

## 📄 Licença
GPLv3

---

## 👨‍💻 Autor
Criado por [Caio Delgado](https://linktr.ee/caiodelgadonew)  
Adaptações e melhorias para **openSUSE** por [Emerson Silva](https://github.com/silvemerson)  

> Contribuições são muito bem-vindas! Faça um *fork* e envie seu *pull request*.