# 影の剣 Kage no Ken — Lâmina das Sombras

Jogo de ação samurai em 3D, em terceira pessoa, no estilo Sekiro (postura, deflexão, golpe final), que roda direto no navegador, no celular ou no PC.

Cinco mundos abertos inspirados nas obras de **André Wenningkamp**:

| Mundo | Obra | Chefe |
|---|---|---|
| 小鳥 | Passarinho | Gavião Cinzento |
| 海 | Quero o mar, mãe | Ronin da Maré |
| 真 | A verdade | O Mascarado |
| 祈 | Oração | Monge do Silêncio |
| 影 | Eu e a sombra | A Sombra |

## Como jogar

- **Android:** baixe o `KageNoKen.apk` na aba [Releases](../../releases/latest) e instale. O APK é gerado automaticamente pelo GitHub Actions a cada atualização. Ele roda offline e em tela cheia.
- **Navegador:** acesse https://andreluis29.github.io/kage-no-ken/ ou abra o `index.html`.

- **Combate:** combo de 4 golpes, golpe forte carregado, deflexão perfeita e contra-golpe, investida, mergulho aéreo e 6 artes da espada.
- **Progressão:** katana, armadura e amuleto em 5 raridades, com atributos aleatórios, forja até +10, desmanche e relíquias únicas.
- **Mundo:** mapas abertos com raio de 200 m, 2 santuários, 14 acampamentos, 16 baús e minimapa, além de arenas com três provações.
- **Masmorras:** duas por mundo, geradas por algoritmo, com salas, corredores, tochas e o Guardião das Profundezas no fim.
- **Trajes:** 11 trajes desbloqueáveis por conquistas (vencer arenas, abrir baús, conquistar masmorras, usar o domínio, completar ciclos).
- **Ultimate:** expansão de domínio 領域展開. Cada mundo tem o seu domínio: Céu dos Mil Pássaros, Maré da Mãe, Salão dos Espelhos da Verdade, Templo da Oração Silenciosa e Abismo: Eu e a Sombra.
- **Visual:** shaders exagerados com bloom, raios de sol, contorno de tinta e aberração cromática. Também há modo deus.

### Controles (PC)
WASD mover · Mouse câmera · Clique esq. combo · E (segurar) golpe forte · Clique dir. defender/defletir · Shift esquiva · Espaço pulo · Q arte · V domínio · R cabaça · F travar · X interagir · I inventário · G modo deus

No celular, os controles aparecem na tela (joystick e botões).

## Estrutura
- `index.html`: o jogo inteiro (three.js + shaders próprios)
- `android/`: app Android (WebView em tela cheia) que empacota o jogo
- `.github/workflows/apk.yml`: compila e assina o APK e publica como Release
- `.github/workflows/pages.yml`: publica a versão web no GitHub Pages

Feito com [three.js](https://threejs.org/).
