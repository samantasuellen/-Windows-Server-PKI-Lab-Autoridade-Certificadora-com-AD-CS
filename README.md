## 🎯 Objetivos de Aprendizado

- Instalar e configurar o **AD CS (Active Directory Certificate Services)**
- Criar e gerenciar uma **Enterprise Root CA**
- Configurar **templates de certificados** personalizados
- Distribuir certificados automaticamente via **autoenrollment (GPO)**
- Entender a cadeia de confiança de uma **PKI corporativa**

---

## 🗂️ Estrutura do Repositório

```
windows-server-pki-lab/
├── docs/
│   ├── 01-instalacao-AD-CS.md        # Instalação da Autoridade Certificadora
│   └── 02-emissao-certificados.md    # Emissão e distribuição de certificados
├── screenshots/
│   ├── ca-instalada.png              # (adicione suas capturas de tela aqui)
│   └── certificado-emitido.png
└── README.md
```

---

## 🖥️ Topologia do Ambiente

| Componente | Detalhes |
|---|---|
| Sistema Operacional | Windows Server 2022 |
| Endereço IP (Servidor) | 192.168.98.20 |
| Domínio AD | aluno.hacker.com |
| Nome da CA | aluno-DC01-CA |
| Tipo de CA | Enterprise Root CA |
| Algoritmo de chave | RSA 2048 bits |
| Hash | SHA256 |
| Validade dos certificados | 10 anos |

---

## 📚 Documentação

### Instalação da Autoridade Certificadora
Configuração do AD CS no Windows Server 2022, criando uma Enterprise Root CA integrada ao Active Directory.

👉 [Ver documentação completa](docs/01-instalacao-AD-CS.md)

### Emissão de Certificados Digitais
Criação de templates personalizados, configuração de GPO para autoenrollment e emissão automática de certificados para os clientes da rede.

👉 [Ver documentação completa](docs/02-emissao-certificados.md)

---

## 🔑 Conceitos Abordados

- **PKI (Public Key Infrastructure)** — infraestrutura de chaves públicas
- **CA (Certificate Authority)** — autoridade certificadora
- **Certificados digitais** — emissão, gerenciamento e revogação
- **Active Directory** — integração com domínio corporativo
- **Group Policy (GPO)** — distribuição automatizada de certificados
- **Criptografia assimétrica** — RSA 2048 + SHA256
- **Autoenrollment** — inscrição automática de certificados

---

## ⚠️ Aviso

O ambiente descrito é um laboratório isolado. Todas as credenciais e endereços IP presentes na documentação são fictícios ou de uso exclusivo em ambiente controlado. **Nunca utilize estas configurações em ambientes de produção sem as devidas adaptações de segurança.**

---

## 📄 Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

