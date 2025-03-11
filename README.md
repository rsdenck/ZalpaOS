# ZalpaOS

<p align="center">
  <img src="https://github.com/rsdenck/ZalpaOS/blob/main/icon/ZalpOS.png" alt="ZalpaOS" />
</p>

**ZalpaOS** é um sistema operacional baseado no **Alpine Linux**, otimizado para ser um **Appliance do Zabbix Proxy 7.0** com foco em segurança, performance e simplicidade. Este projeto oferece uma ISO minimalista com Zabbix Proxy pronto para ser utilizado em ambientes de monitoramento de infraestruturas, combinando leveza e criptografia de ponta.

## 🚀 **O que é o ZalpaOS?**

O **ZalpaOS** é um sistema operacional **compacto** e **eficiente** com o **Zabbix Proxy 7.0** integrado, projetado para ser utilizado em ambientes de monitoramento distribuído. A ISO é baseada no **Alpine Linux**, um sistema operacional com baixíssimo consumo de recursos, tornando-o ideal para máquinas com recursos limitados ou para grandes implantações com alto desempenho.

### 🔐 **Segurança e Criptografia de Ponta**
- **Criptografia PSK-SHA-512** para garantir uma comunicação segura entre o Zabbix Proxy e o Zabbix Server.
- **SQLCipher** é utilizado para criptografar o banco de dados **SQLite-3**, protegendo os dados contra interceptações (sniffing) e garantindo a segurança de dados armazenados.
- **Desabilitação do usuário root** para conexões SSH, aumentando a segurança do sistema e prevenindo acessos não autorizados.

## 🌟 **Principais Características**
- **Baseado no Alpine Linux**: Leve e altamente eficiente, com baixo consumo de **RAM (20-50 MB)** e **CPU (menos de 1%)**.
- **Zabbix Proxy 7.0** pronto para uso, configurado para fácil implementação em ambientes de monitoramento.
- **Criptografia de dados** com **PSK SHA-512** e **SQLCipher** para garantir a proteção de dados em repouso e em trânsito.
- **ISO Minimalista**: Apenas os pacotes necessários, permitindo uma instalação rápida e eficiente.
- **Desabilitação de root** para conexões SSH, aumentando a segurança do sistema.

## 💻 **Como Usar o ZalpaOS?**

### **1. Baixar a ISO**
Acesse o repositório e baixe a ISO mais recente do ZalpaOS para começar a usar o Zabbix Proxy em seu ambiente.

- [Baixar ISO do ZalpaOS](https://github.com/rsdenck/ZalpaOS/releases)

### **2. Criar um Ambiente Virtual ou Física**
- Crie uma máquina virtual ou utilize um dispositivo físico para hospedar o **ZalpaOS**.
- O sistema foi otimizado para ser leve, funcionando bem em máquinas com recursos limitados.

### **3. Configurar Zabbix Proxy**
- Após a instalação, o **Zabbix Proxy** será configurado automaticamente para se comunicar com o **Zabbix Server**.
- **PSK-SHA-512** já estará configurado para garantir segurança na comunicação.
- O banco de dados SQLite3 será criptografado com SQLCipher, protegendo seus dados.

### **4. Acesse o Sistema**
- O Zabbix Proxy estará pronto para uso, com a interface de configuração padrão do Zabbix para gerenciar o monitoramento.

## 🔧 **Configurações Avançadas**
Você pode personalizar a configuração do Zabbix Proxy e ajustar as configurações de criptografia conforme necessário. Consulte o arquivo de configuração do Zabbix Proxy para mais informações detalhadas.

```bash
# Editar configuração do Zabbix Proxy
vi /etc/zabbix/zabbix_proxy.conf
