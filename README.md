# TelegramCMD
Envio de mensagens para o telegram por meio de shell script para grupo <br>

<b>Requerimentos</b>

Debian/Ubuntu:
<pre>apt install curl wget zip</pre>

CentOS / Fedora / Red hat
<pre>yum install curl wget zip</pre>

<b>Instalacação:</b>
<pre>cd /tmp/
wget https://github.com/remontti/TelegramCMD/archive/master.zip
unzip /tmp/master.zip
chmod 777 /tmp/TelegramCMD-master/telegram
mv /tmp/TelegramCMD-master/telegram* /usr/local/bin/</pre>

<b>Modelo de uso:</b>

- -m: Para enviar uma mensagem
<pre>telegram -m "ID Chat" "Meu assunto" "Minha mensagem..."
telegram -m "123456789" "Notificação" "Ataque identificado"</pre>

- -f: Para enviar um arquivo (o memos será zipado)
<pre>telegram -f "ID Chat" "/diretorio/arquivo" "nome do arquivo zip" "Comentário"
telegram -f 12345689 /var/log/syslog syslog "Logs do sistema"</pre>
