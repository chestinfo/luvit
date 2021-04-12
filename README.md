# Example file for discordia
local discordia = require('discordia')
local client = discordia.Client()

client:on('ready', function()
	print('Logged in as '.. client.user.username)
end)

client:on('messageCreate', function(message)
	if message.content == '!ping' then
		message.channel:send('Pong!')
	end
end)

client:run('Bot INSERT_BOT_TOKEN_HERE')

# Komenda do instalacji luvita
Aby zainstalować luvit należy utworzyć folder na pulpicie o wybranej nazwie np. luvit
Potem należy w wyszukiwaniu windows wpisać cmd i uruchomić program
Następnie wpisać: cd C:\Users\User\Desktop\nazwa-utworzonego-folderu
Kliknąć enter i wkleić tą komendę:

DLA WINDOWS:
PowerShell -NoProfile -ExecutionPolicy unrestricted -Command "[Net.ServicePointManager]::SecurityProtocol = 'Tls12'; iex ((new-object net.webclient).DownloadString('https://github.com/luvit/lit/raw/master/get-lit.ps1'))"

DLA LINUX (tylko komenda poradnika nie ma)
curl -L https://github.com/luvit/lit/raw/master/get-lit.sh | sh

Kliknąć enter i gotowe!

# Instalacja discordia (wymagane do luvit)
Aby zainstalować Discordia.Local.Client należy:
1. Utworzyć folder na pulpicie o wybranej nazwie np. luvit
2. W wyszukiwaniu windows wpisać cmd i uruchomić program
3. wpisać: cd C:\Users\User\Desktop\nazwa-utworzonego-folderu
4. Kliknąć enter i wkleić tą komendę:
       lit install SinisterRectus/discordia
       
# Uruchamianie bota
Nie chce mi się pisać więc jest link do poradnika: https://www.youtube.com/watch?v=PhblU286UlY
