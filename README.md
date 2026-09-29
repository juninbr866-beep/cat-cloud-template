<div align="center">

# 🐱 Cat Cloud

**PC Windows grátis, rodando dentro do GitHub Actions, acessível por RDP.**

Sem servidor. Sem cartão. Sem custo pra você.

[**▶️ Criar minha sessão**](https://github.com/juninbr866-beep/cat-cloud-template/generate) &nbsp;·&nbsp;
[**Como funciona**](#-como-funciona) &nbsp;·&nbsp; [**Requisitos**](#-requisitos)

</div>

---

## O que é

O GitHub te empresta um Windows completo por algumas horas. A gente liga o Remote Desktop,
liga uma VPN, e te entrega o endereço. Você conecta de casa, do celular, de qualquer lugar.

- **Windows Server 2022** ou 2019, ou o Windows 11 mais recente
- **Remote Desktop** com NLA
- **Acesso por VPN** — sua máquina não fica exposta na internet aberta
- **Duração configurável**, de 15 a 180 minutos
- **Sem conta, sem senha, sem cadastro** neste repositório

## Como funciona em 3 passos

**1.** Crie sua sessão aqui em cima, no botão verde. Isso abre o GitHub com o template
pronto pra você aceitar.

**2.** No seu repo novo, abra a aba **Actions**, escolha o workflow **Cat Cloud** e clique
em **Run workflow**.

**3.** Cole o **token de sessão** que o site te deu, escolha quantos minutos, e rode.

Em uns 2 a 3 minutos a máquina está de pé. O site mostra o IP e a senha.

## Requisitos

Só isso:

- Uma conta no **GitHub** (a conta_free serve, e todo mundo tem)
- Um **token de sessão**, que você pega no site antes de começar
- **Tailscale** instalado no seu PC ou celular, porque a conexão é por VPN

Nada de configuração de VPN, nada de chave SSH, nada de segredo. O token da sessão é o
único dado que você digita.

## O que acontece com a sua cota

Cada sessão roda **no seu próprio GitHub**, então o tempo sai da cota **sua**, não da nossa.
Conta gratuita do GitHub vem com 2.000 minutos por mês. No Windows, cada minuto conta como
dois, então dá para umas 16 sessões de uma hora, ou umas 50 sessões curtas de 20 minutos.

A máquina é destruída quando o tempo acaba. Nada fica salvo.

## Perguntas

**É de graça mesmo?**
Sim. Não cobramos, não pedimos cartão, não pedimos cadastro. O custo de computação é da
conta do GitHub de quem usa.

**A máquina some mesmo?**
Sim. Quando o tempo acaba, o workflow termina, a VM é destruída e o acesso some junto. Nada
do que você fizer fica salvo em lugar nenhum.

**Dá pra eu confiar?**
O código do workflow está todo neste repositório, você pode ler antes de rodar. Ele pede
um token de sessão pro nosso servidor e executa o script de provisionamento que o servidor
devolve. A chave de acesso nunca fica neste repositório.

**Posso rodar várias vezes?**
Pode, respeitando a cota da sua conta. Cada sessão é independente.

## Privacidade

O que nosso servidor sabe sobre você:

- o **token de sessão**, que vale para uma sessão e expira sozinho
- o **email ou identificador** que você usar para pedir o token, se usar
- o **IP da máquina** enquanto a sessão está viva, para te mostrar na tela

O que **não** fazemos: guardar senha da sua máquina depois que a sessão acaba, guardar
conteúdo do que você faz dentro da VM, ou vender dado pra terceiros.

A sessão é temporária e some quando você desliga.

---

<div align="center">

**Cat Cloud** · PC na nuvem, sem gastar nada

[Issues](https://github.com/juninbr866-beep/cat-cloud-template/issues)

</div>
