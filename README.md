

## 🖥️ Criação da Máquina Virtual (VM)

1. **Acesso ao portal Azure:** Utilizamos o portal [https://portal.azure.com](https://portal.azure.com) para gerenciar os recursos.
2. **Criação da VM:** Escolhemos a imagem do sistema operacional (Linux/Windows), definimos o nome da máquina, região e tamanho.
3. **Segurança e autenticação:** Configuramos usuário e senha (ou chave SSH), além das regras de acesso via portas (como RDP ou SSH).
4. **Rede e armazenamento:** Ajustamos as configurações de rede virtual, sub-rede, IP público e tipo de disco.

---

## 🔐 Conexão e Configuração da VM

- Após a implantação, acessamos a VM via RDP ou SSH, dependendo do SO.
- Instalamos os softwares necessários (ex: Apache, Nginx, etc).
- Fizemos ajustes de segurança, incluindo atualizações do sistema e configurações de firewall.

---

## ⚖️ Implementação do Balanceador de Carga

Para garantir maior disponibilidade e distribuir o tráfego entre instâncias, configuramos um **Load Balancer**:

1. **Criação do recurso:** Selecionamos um balanceador público.
2. **Pool de backend:** Adicionamos as VMs criadas ao grupo de balanceamento.
3. **Regras de tráfego:** Definimos portas e protocolos de entrada e saída.
4. **Verificações de integridade:** Configuramos sondas para verificar se as VMs estão ativas antes de redirecionar o tráfego.

---

## 📈 Monitoramento e Escalabilidade

- Com o **Azure Monitor**, acompanhamos o desempenho das VMs e do balanceador.
- Criamos alertas para identificar falhas ou picos de uso.
- Estudamos também a possibilidade de usar **VM Scale Sets** para escalar automaticamente os recursos com base na demanda.

---

## ✅ Resultado Final

A estrutura criada permite que múltiplas VMs atendam usuários de forma equilibrada, aumentando a tolerância a falhas e melhorando o desempenho da aplicação.

---

## 📚 Recursos Complementares

- [Portal do Azure](https://portal.azure.com)
- [Documentação oficial de Máquinas Virtuais](https://learn.microsoft.com/pt-br/azure/virtual-machines/)
---

## 🧠 Aprendizado

Esta prática mostrou como iniciar do zero no Azure, estruturando um ambiente robusto com VMs e distribuição de carga. Um passo essencial para quem busca hospedar aplicações com alta disponibilidade em nuvem.

