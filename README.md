# VPN Hub

App para macOS que mantém várias VPNs de clientes ligadas ao mesmo tempo, cada uma isolada no próprio
container (OpenVPN, FortiClient SSL e IPsec, WireGuard e SonicWall NetExtender). Este repositório tem só os
instaladores; o uso depende de uma conta liberada pelo administrador.

## Baixar

**[VPN-Hub.dmg](https://github.com/pedroakbar/vpn-hub-releases/releases/latest/download/VPN-Hub.dmg)**:
última versão, Apple Silicon e Intel, macOS 14 ou mais novo.

1. Abra o `.dmg` e arraste o **VPN Hub** para **Aplicativos**.
2. Na primeira vez, o macOS pode dizer que não consegue verificar o app. Abra **Ajustes do Sistema ›
   Privacidade e Segurança**, role até o aviso do VPN Hub e clique em **Abrir Mesmo Assim**.
3. Crie a sua conta no app e aguarde a liberação.

Na primeira VPN, o app cria a máquina virtual onde as VPNs rodam (precisa de internet e leva alguns
minutos). Não é preciso instalar mais nada: Colima, Lima e Docker vêm dentro do app.

## Atualizações

O app procura versões novas sozinho (ao abrir e a cada 6 horas), baixa e instala quando você fecha o app,
ou na hora, em **Reiniciar** no aviso da barra lateral. Também pelo menu **Hub**, na barra do app, ou por
**VPN Hub › Verificar atualizações…**. As VPNs continuam ligadas durante a troca.

Cada versão traz um `atualizacao.json` assinado; o app só instala o pacote cuja assinatura e SHA-256
conferem.
