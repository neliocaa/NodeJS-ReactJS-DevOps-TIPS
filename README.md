# NodeJS-ReactJS-DevOps-TIPS
## Dicas, Rascunho, e outros códigos úteis, ou não!
<hr>

PM2 com erro ao executar nodejs no usuario padrão (não root)
> Error: listen EACCES: permission denied 0.0.0.0:xxx

Solução:

```
sudo pm2 kill
sudo npm remove pm2 -g

sudo npm i -g pm2@latest
sudo pm2 update
sudo chown -R ubuntu:ubuntu /home/ubuntu/.pm2
```
