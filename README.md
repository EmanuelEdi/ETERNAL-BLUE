# Exploração da Vulnerabilidade EternalBlue em Máquina TryHackMe

## Descrição do Projeto
Este projeto documenta a exploração de uma máquina vulnerável no **TryHackMe** utilizando o exploit **EternalBlue**. O EternalBlue é uma vulnerabilidade crítica no protocolo **SMBv1 (Server Message Block)** do Windows, identificada como **CVE-2017-0144**, que permite a execução remota de código. Este exploit foi originalmente desenvolvido pela **NSA** e vazado pelo grupo **Shadow Brokers** em 2017. 

A exploração demonstrada neste README foi conduzida **para fins educacionais e de aprendizado em segurança cibernética**.

---

## Informações Técnicas

### Vulnerabilidade
- **Nome:** EternalBlue  
- **CVE:** MS17-010  
- **Protocolo Afetado:** SMBv1 (Server Message Block)  
- **Porta Padrão:** TCP 445  
- **Impacto:** Execução remota de código, comprometendo completamente o sistema alvo.  

---

### Descrição Técnica
O **EternalBlue** explora uma falha no gerenciamento de pacotes SMBv1 especialmente formatados. Um atacante pode enviar pacotes maliciosos ao servidor SMB vulnerável, permitindo a execução arbitrária de código e, potencialmente, o movimento lateral na rede.

Esta vulnerabilidade foi usada em ataques notórios como **WannaCry** e **NotPetya**, que causaram prejuízos globais significativos.

## Medidas de Mitigação

Para proteger sistemas contra ataques similares ao **EternalBlue**, recomenda-se:

- **Aplicar patches de segurança:** Instale o patch **MS17-010** disponibilizado pela Microsoft.  
- **Desabilitar SMBv1:** Utilize versões mais seguras do protocolo, como **SMBv2** ou **SMBv3**.  
- **Segmentação de rede:** Restrinja o tráfego SMB apenas para dispositivos autorizados.  
- **Monitoramento ativo:** Configure sistemas **IDS/IPS** para detectar atividades suspeitas na porta 445.  
- **Educação e conscientização:** Treine equipes para identificar sinais de ataques cibernéticos.  

---

## Ferramentas Utilizadas

- **Nmap:** Para reconhecimento e verificação de vulnerabilidades.  
- **Metasploit Framework:** Para exploração da vulnerabilidade.  
- **John The Ripper:** Para quebra de hash.  

---
#Link Explicação
https://pyrite-principle-7f8.notion.site/ETERNAL-BLUE-18057605a28b803f8eb8fb1e1eb175ac

## Conclusão

A exploração da vulnerabilidade **EternalBlue** demonstrou a importância crítica da aplicação de patches e boas práticas de segurança. Mesmo anos após seu vazamento, sistemas desatualizados continuam sendo alvos fáceis para ataques cibernéticos. Este exercício reforça a necessidade de uma gestão proativa de vulnerabilidades em ambientes corporativos e educacionais.

---

### Nota
Este projeto foi realizado exclusivamente em um ambiente controlado e autorizado no **TryHackMe**, respeitando os princípios éticos da segurança cibernética.

---

## Referências
1. Wikipedia sobre EternalBlue  
2. SentinelOne: Como funciona o EternalBlue  
3. NordVPN: Explicação técnica do EternalBlue  
4. TrendMicro: Impacto contínuo do EternalBlue
