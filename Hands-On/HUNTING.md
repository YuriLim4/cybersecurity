# 🔎 OSINT  

**Open Source intelligence**  

Este espaço é dedicado ao meu aprendizado em **OSINT**. Aqui vou tentar concatenar conceitos, links úteis e etc...  

---

## ❓ O QUE É OSINT?   
- **Conceito Geral**: Utilização de fontes públicas para pesquisa e coleta de informações.  
- **Aplicabilidade**: Coleta de informações "rasas ou não" de um indivíduo com a finalidade ética de conhecimento.

---

## ▶ Começando  
**Vamos imaginar o seguinte caso:**

Você atua na empresa X, uma organização inserida em um mercado altamente competitivo e em constante ascensão tecnológica. Cada avanço inovador, por menor que pareça, posiciona a empresa como referência seja para investidores estratégicos ou veículos de mídia especializados.

Contudo, a diretoria observou que informações estratégicas relacionadas a decisões de inovação têm se tornado públicas com agilidade incomum, muitas vezes sendo rapidamente replicadas por concorrentes diretos. Essa coincidência reiterada levanta uma suspeita concreta de vazamento de informações confidenciais.

Ao invés de gerar alarde, a empresa optou por uma abordagem silenciosa e estratégica: acionar o time de Cybersecurity para iniciar uma operação de Threat Hunting. A missão é clara, identificar se há, de fato, um vazamento interno, mapear as possíveis origens e detectar padrões ou pontos frágeis no fluxo de informações sensíveis.

Agora você entra na primeira camada da caçada:

- Coletar dados

- Analisar comportamentos suspeitos

- Mapear possíveis canais de exposição

- Identificar inconsistências em acessos e comunicações

- Investigar sinais de engenharia social ou exfiltração sutil de dados

Esse é o início de um caso real de investigação digital, onde seu papel como hunter é essencial para preservar a integridade e a vantagem competitiva da empresa.

---

## 🌐 Contas em Sites

Na etapa inicial da investigação, você terá acesso a um conjunto de dados que podem ou não ser imediatamente relevantes. Entre esses dados, é comum encontrar informações como fotos, nome completo, CPF, e-mail, número de telefone, entre outros.

Mesmo que pareçam triviais, esses elementos podem servir como ponto de partida estratégico para uma busca mais aprofundada, especialmente em redes sociais e plataformas públicas.

Um comportamento recorrente entre usuários é o reuso de identificadores, como usernames e e-mails, em diferentes serviços. Isso significa que, ao identificar um e-mail como jhondoe@gmail.com, há uma alta probabilidade de que o mesmo identificador (ou variações próximas) esteja sendo utilizado em perfis de redes sociais, fóruns, serviços de streaming, marketplaces, entre outros.

Esse tipo de padrão comportamental pode ser explorado para correlação de identidades digitais, facilitando a ampliação da coleta de dados dentro de um processo de OSINT.

Aqui utilizei a ferramenta [Sherlock](https://www.kali.org/tools/sherlock/). Dentro do OS Kali Linux.
```                                                                                            
┌──(root㉿kali)-[/home/neo]
└─# sherlock jhondoe
[*] Checking username jhondoe on:

[+] 7Cups: https://www.7cups.com/@jhondoe
[+] 9GAG: https://www.9gag.com/u/jhondoe
[+] About.me: https://about.me/jhondoe
[+] AllMyLinks: https://allmylinks.com/jhondoe
[+] Apple Discussions: https://discussions.apple.com/profile/jhondoe
[+] Asciinema: https://asciinema.org/~jhondoe
[+] Bandcamp: https://www.bandcamp.com/jhondoe
[+] Behance: https://www.behance.net/jhondoe
[+] BitBucket: https://bitbucket.org/jhondoe/
[+] BuyMeACoffee: https://buymeacoff.ee/jhondoe
[+] BuzzFeed: https://buzzfeed.com/jhondoe
[+] Chess: https://www.chess.com/member/jhondoe
[+] Clapper: https://clapperapp.com/jhondoe
[+] Clubhouse: https://www.clubhouse.com/@jhondoe
[+] Codecademy: https://www.codecademy.com/profiles/jhondoe
[+] Codechef: https://www.codechef.com/users/jhondoe
[+] Crowdin: https://crowdin.com/profile/jhondoe
[+] Cults3D: https://cults3d.com/en/users/jhondoe/creations
[+] DeviantART: https://jhondoe.deviantart.com
[+] DigitalSpy: https://forums.digitalspy.com/profile/jhondoe
[+] Discord: https://discord.com
[+] Disqus: https://disqus.com/jhondoe
[+] Docker Hub: https://hub.docker.com/u/jhondoe/
[+] Dribbble: https://dribbble.com/jhondoe
[+] Duolingo: https://www.duolingo.com/profile/jhondoe
[+] EyeEm: https://www.eyeem.com/u/jhondoe
[+] Flickr: https://www.flickr.com/people/jhondoe
[+] Flipboard: https://flipboard.com/@jhondoe
[+] Freelance.habr: https://freelance.habr.com/freelancers/jhondoe
[+] Freelancer: https://www.freelancer.com/u/jhondoe
[+] Freesound: https://freesound.org/people/jhondoe/
[+] GNOME VCS: https://gitlab.gnome.org/jhondoe
[+] Genius (Users): https://genius.com/jhondoe
[+] GitHub: https://www.github.com/jhondoe
[+] GitLab: https://gitlab.com/jhondoe
[+] Gitee: https://gitee.com/jhondoe
[+] Grailed: https://www.grailed.com/jhondoe
[+] Gumroad: https://www.gumroad.com/jhondoe
[+] Gutefrage: https://www.gutefrage.net/nutzer/jhondoe
[+] Hackaday: https://hackaday.io/jhondoe
[+] HackerNews: https://news.ycombinator.com/user?id=jhondoe
[+] HackerRank: https://hackerrank.com/jhondoe
[+] Houzz: https://houzz.com/user/jhondoe
[+] HubPages: https://hubpages.com/@jhondoe
[+] HudsonRock: https://cavalier.hudsonrock.com/api/json/v2/osint-tools/search-by-username?username=jhondoe
[+] Hugging Face: https://huggingface.co/jhondoe
[+] Imgur: https://imgur.com/user/jhondoe
[+] Instructables: https://www.instructables.com/member/jhondoe
[+] Itch.io: https://jhondoe.itch.io/
[+] kaskus: https://www.kaskus.co.id/@jhondoe
[+] Keybase: https://keybase.io/jhondoe
[+] Kongregate: https://www.kongregate.com/accounts/jhondoe
[+] Launchpad: https://launchpad.net/~jhondoe
[+] Letterboxd: https://letterboxd.com/jhondoe
[+] LibraryThing: https://www.librarything.com/profile/jhondoe
[+] Lichess: https://lichess.org/@/jhondoe
[+] Linktree: https://linktr.ee/jhondoe
[+] Medium: https://medium.com/@jhondoe
[+] Memrise: https://www.memrise.com/user/jhondoe/
[+] Monkeytype: https://monkeytype.com/profile/jhondoe
[+] MyAnimeList: https://myanimelist.net/profile/jhondoe
[+] MyMiniFactory: https://www.myminifactory.com/users/jhondoe
[+] Mydramalist: https://www.mydramalist.com/profile/jhondoe
[+] Myspace: https://myspace.com/jhondoe
[+] NationStates Nation: https://nationstates.net/nation=jhondoe
[+] NationStates Region: https://nationstates.net/region=jhondoe
[+] Newgrounds: https://jhondoe.newgrounds.com
[+] NitroType: https://www.nitrotype.com/racer/jhondoe
[+] OpenStreetMap: https://www.openstreetmap.org/user/jhondoe
[+] Pastebin: https://pastebin.com/u/jhondoe
[+] Patreon: https://www.patreon.com/jhondoe
[+] Periscope: https://www.periscope.tv/jhondoe/
[+] Pokemon Showdown: https://pokemonshowdown.com/users/jhondoe
[+] Polarsteps: https://polarsteps.com/jhondoe
[+] ProductHunt: https://www.producthunt.com/@jhondoe
[+] Redbubble: https://www.redbubble.com/people/jhondoe
[+] Reddit: https://www.reddit.com/user/jhondoe
[+] ReverbNation: https://www.reverbnation.com/jhondoe
[+] Scratch: https://scratch.mit.edu/users/jhondoe
[+] Scribd: https://www.scribd.com/jhondoe
[+] Sketchfab: https://sketchfab.com/jhondoe
[+] Slack: https://jhondoe.slack.com
[+] SlideShare: https://slideshare.net/jhondoe
[+] Slides: https://slides.com/jhondoe
[+] Smule: https://www.smule.com/jhondoe
[+] SoundCloud: https://soundcloud.com/jhondoe
[+] Speedrun.com: https://speedrun.com/users/jhondoe
[+] Sporcle: https://www.sporcle.com/user/jhondoe/people
[+] Spotify: https://open.spotify.com/user/jhondoe
[+] Star Citizen: https://robertsspaceindustries.com/citizens/jhondoe
[+] Steam Community (Group): https://steamcommunity.com/groups/jhondoe
[+] Steam Community (User): https://steamcommunity.com/id/jhondoe/
[+] TETR.IO: https://ch.tetr.io/u/jhondoe
[+] Tiendanube: https://jhondoe.mitiendanube.com/
[+] Topcoder: https://profiles.topcoder.com/jhondoe/
[+] Telegram: https://t.me/jhondoe
[+] Tenor: https://tenor.com/users/jhondoe
[+] TorrentGalaxy: https://torrentgalaxy.to/profile/jhondoe
[+] TradingView: https://www.tradingview.com/u/jhondoe/
[+] Trello: https://trello.com/jhondoe
[+] TryHackMe: https://tryhackme.com/p/jhondoe
[+] Twitter: https://x.com/jhondoe
[+] Typeracer: https://data.typeracer.com/pit/profile?user=jhondoe
[+] Ultimate-Guitar: https://ultimate-guitar.com/u/jhondoe
[+] Unsplash: https://unsplash.com/@jhondoe
[+] Untappd: https://untappd.com/user/jhondoe
[+] VK: https://vk.com/jhondoe
[+] VSCO: https://vsco.co/jhondoe
[+] VirusTotal: https://www.virustotal.com/gui/user/jhondoe
[+] Warrior Forum: https://www.warriorforum.com/members/jhondoe.html
[+] Wattpad: https://www.wattpad.com/user/jhondoe
[+] Weblate: https://hosted.weblate.org/user/jhondoe/
[+] Wikidot: http://www.wikidot.com/user:info/jhondoe
[+] Wikipedia: https://en.wikipedia.org/wiki/Special:CentralAuth/jhondoe?uselang=qqx
[+] WordPress: https://jhondoe.wordpress.com/
[+] WordPressOrg: https://profiles.wordpress.org/jhondoe/
[+] Xbox Gamertag: https://xboxgamertag.com/search/jhondoe
[+] YandexMusic: https://music.yandex/users/jhondoe/playlists
[+] YouNow: https://www.younow.com/jhondoe/
[+] YouTube: https://www.youtube.com/@jhondoe
[+] couchsurfing: https://www.couchsurfing.com/people/jhondoe
[+] dailykos: https://www.dailykos.com/user/jhondoe
[+] datingRU: http://dating.ru/jhondoe
[+] devRant: https://devrant.com/users/jhondoe
[+] eGPU: https://egpu.io/forums/profile/jhondoe/
[+] furaffinity: https://www.furaffinity.net/user/jhondoe
[+] geocaching: https://www.geocaching.com/p/default.aspx?u=jhondoe
[+] interpals: https://www.interpals.net/jhondoe
[+] jbzd.com.pl: https://jbzd.com.pl/uzytkownik/jhondoe
[+] jeuxvideo: https://www.jeuxvideo.com/profil/jhondoe
[+] kofi: https://ko-fi.com/jhondoe
[+] kwork: https://kwork.ru/user/jhondoe
[+] last.fm: https://last.fm/user/jhondoe
[+] minds: https://www.minds.com/jhondoe/
[+] note: https://note.com/jhondoe
[+] npm: https://www.npmjs.com/~jhondoe
[+] osu!: https://osu.ppy.sh/users/jhondoe
[+] pikabu: https://pikabu.ru/@jhondoe
[+] Bluesky: https://bsky.app/profile/jhondoe.bsky.social
```
Aqui conseguimos identificar o mesmo username em diversos sites. E possível que haja informações nesses sites que podemos utilizar. Fotos, comentários, aplicações para vagas ou até mesmo os podcasts que a pessoa escuta podem ter relação com aquilo que você procura.

Vamos imaginar que ele acessa redes sociais como Twitter, Facebook, Reddit e Medium. Utilizando outra técnica como Google Dorks, vamos pesquisar o seguinte texto na barra de pesquisa do google.
```
intext:"jhondoe" inurl:https://medium.com
```
Aqui teremos todas as informações sobre jhondoe dentro do site Medium. Porém, caso nossa hunt seja referente a um vazamento dos arquivos XYZ. Nosso prompt então seria assim:
```
intext:"jhondoe""XYZ" inurl:https://medium.com
```
Dessa forma, o google buscará tudo indexado com as palavras jhondoe e XYZ. 

>*Mas e claro que você entendeu que esse processo que estamos fazendo, está totalmente fictício.*

---

## 🤝 Contribuições & Feedback  
Encontrou algo incorreto ou tem sugestões? **Adoraria ouvir você!**  
- Abra uma **issue** ou envie um **pull request**.  
- Conecte-se comigo no [LinkedIn](https://linkedin.com/in/yurilim4).  

--- 

📌 *"Knowledge shared is knowledge squared."*  
