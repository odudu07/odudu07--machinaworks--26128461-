# MachinaWorks – Deploy Cloud

Projeto estático HTML/CSS/JavaScript preparado para o LAB6 – Cloud.

## Render.com (PaaS)
- Tipo: Static Site
- Build Command: vazio
- Publish Directory: vazio
- O arquivo `index.html` está na raiz do projeto.

## AWS EC2 (IaaS)
Ubuntu Server LTS + Apache.

```bash
sudo apt update
sudo apt install apache2 -y
sudo systemctl enable --now apache2
```

Depois, copie o conteúdo deste diretório para `/var/www/html/` e acesse:
`http://SEU_IP_PUBLICO`

Security Group:
- HTTP 80 → Anywhere
- SSH 22 → My IP

## Desafio
Foi feita uma alteração pequena no HTML: título e texto principal foram atualizados para MachinaWorks/Dashboard Industrial. Faça commit/push dessa alteração para o GitHub e observe o redeploy automático no Render.

## Observação
As capturas de tela com IP público do EC2 e URL real do Render precisam ser feitas após o deploy nas respectivas contas; não foram simuladas neste pacote.
